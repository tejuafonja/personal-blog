---
title: One-hot Encoding
date: 2021-05-19T11:29:00.946Z
published: true
tags:
  - programming
  - python
  - numpy
description: Did you know that one-hot encoding in digital circuitry is often
  used to indicate the state of a state machine?
---
Hmmn! Now the name makes perfect sense, considering that in Machine Learning we often use this term to encode the categorical feature, so we don't really assign any meaning to the individual classes of the feature. Individually, the class category can be thought of as a state which is either on (1) or off (0).

What is One-Hot Encoding?

In Machine learning and statistics, one-hot encoding is an encoding technique that is often used to deal with categorical data. This is because many machine learning models need their input variables to be numeric, so we transform the categorical variables into numerical variables. Imagine you have some data with a column called Food Name, this column contains different food name category as described below 

```python
food_name= ["Apple", "Chicken", "Broccoli", "Carrot", "Chicken", "Apple", "Carrot", "Carrot", "Apple"]
```

You can turn this into numerical (one-hot encoding) by doing the following transformation

| Apple <> | Chicken <> | Broccoli <> | Carrot |
| :-----: | :-------:| :------: | :------:|
| 1               | 0                 | 0                  | 0                |
| 0               | 1                 | 0                  | 0                |
| 0               | 0                 | 1                  | 0                |
| 0               | 0                 | 0                  | 1                |
| 0               | 1                 | 0                  | 0                |
| 1               | 0                 | 0                  | 0                |
| 0               | 0                 | 0                  | 1                |
| 0               | 0                 | 0                  | 1                |
| 1               | 0                 | 0                  | 0                |
Table 1: One-hot Encoding Table for Food Name


What we have done here is that we transformed the data in such a way that we input 1 if the category is what we're currently observing, otherwise, we input 0. 

This is all one-hot encoding is doing.

If you want to write the function yourself, checkout this python code snippet below. You can also just use the inbuilt function from [numpy](https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.OneHotEncoder.html) :<p

```python
food_name = ["Apple", "Chicken", "Broccoli", "Carrot", "Chicken", "Apple", "Carrot", "Carrot", "Apple"]

food_name_map = {"Apple": 0, "Chicken": 1, "Broccoli": 2, "Carrot": 3}

y = [food_name_map[i] for i in food_name] 

print(y) # y = [0, 1, 2, 3, 1, 0, 3, 3, 0]

y = np.array(y)

n = y.shape[0]

category = np.zeros((n, len(food_name_map)), dtype=np.float)

print(category)
# array([[0., 0., 0., 0.],
#       [0., 0., 0., 0.], 
#       [0., 0., 0., 0.],
#       [0., 0., 0., 0.],
#       [0., 0., 0., 0.],
#       [0., 0., 0., 0.],
#       [0., 0., 0., 0.],
#       [0., 0., 0., 0.],
#       [0., 0., 0., 0.]])

category[np.arange(n), y] = 1

print(category)
# array([[1., 0., 0., 0.],
#       [0., 1., 0., 0.],
#       [0., 0., 1., 0.],
#       [0., 0., 0., 1.],
#       [0., 1., 0., 0.],
#       [1., 0., 0., 0.],
#       [0., 0., 0., 1.],
#       [0., 0., 0., 1.],
#       [1., 0., 0., 0.]])
```

You can see that this looks exactly like the one-hot encoding in table 1.

That's it for today, folks. If you want to learn more about it, check out the [wiki page](https://www.wikiwand.com/en/One-hot) -:), I hardly understand wiki the first time, but I'm slowly learning that it's the most resourceful material out there, and learning how to read wiki will help you a lot, especially if you're considering graduate school. People here like to cite wiki a lot, understandably. That being said, if you're still having trouble understanding it, feel free to [write me](teju.afonja@aisaturdayslagos.com).

The hashtag is still the same on twitter :P #XhirotByTej