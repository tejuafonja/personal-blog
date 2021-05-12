<template>
    <Layout class="content-box" :show-logo='false'>
        <div class="profile-header">
          <g-image src="~/assets/images/about-img.jpg" class="profile-img"></g-image>
          <h2 >Tẹjúmádé Àfọ̀njá</h2>
        </div>

        
        <div class="intro-box">
            <div>
                <p>Hi there, it's Tejumade Afonja - thanks for visiting. Since you're here, 
		I'd like to invite you to participate in a <a href="bit.ly/accent_influence" target="_blank">short anonymous survey</a> 
		I'm conducting to understand the impact of accent on learning. It will take about 2-5min and I would really appreciate your opinion. 
		If you can also share the survey with your network, that's even more awesome. Thank you so much!
		</p>

                <div>
                    I'm in my 3rd semester of Masters program at Saarland University, studying Computer Science.
                    I'm also remotely working with <a href="https://www.papernot.fr/" target="_blank">Prof. Nicolas Papernot</a> 
                    from the University of Toronto
                    as a research intern where I'm researching the security of Speaker classification models.
                  
                    You can check out <a href="http://www.cleverhans.io/" target="_blank">cleverhans.io</a> 
                    for more details on my research interests. 
                </div>
                <br>
                <div>
                    In 2018, I co-founded <a href="http://www.aisaturdayslagos.com/" target="_blank">AI Saturdays Lagos</a>, 
                    an artificial intelligence community based in Lagos, 
                    Nigeria where we offer free-to-attend classes on Data Science, Machine Learning and 
                    Deep Learning for about 12 - 16 weeks (classes are held on Saturdays) through structured study groups.
                     Our community is one of the largest AI community in Nigeria 
                     and for the past three (3) years, we have been honored to 
                     produce alumni in various academic institutions and IT industries.
                </div>

                <br>
                <div>
                    I've always been passionate and fascinated about Artificial Intelligence (AI) for 
                    as long as I can remember and I believe that AI has potential to improve life without 
                    opening up or exacerbate inequalities but to achieve this, locations in 
                    which AI is done will have to be widened and ambitious goals to democratize AI education 
                    will need to be set. Doing so will allow a broader audience to discuss and contribute to 
                    the success of an AI-enabled world. My team and I are focused on bridging this gap of 
                    Artificial Intelligence in Nigeria through our AI Saturdays Classes.
                </div>

                <br>

                <p>You can stay in touch with me via <a href="https://twitter.com/tejuafonja">Twitter</a>
                and <a href="https://linkedin.com/in/tejumadeafonja">LinkedIn</a>. 
                You can also check out <g-link to='/xhirot'>Xhirot</g-link>, it's where
                I dump my thoughts on topics I'm interested in.</p>
                
        

          
                 
                
            </div>
          <!-- <g-image src="~/assets/images/about-img.jpg" width="400" /></div> -->
        </div>


        <!-- <div>
            <h2>Some side, but very important projects</h2>
            <ul>
                <li>[Podcast] <a href="https://anchor.fm/onequestion">The ONE question podcast</a> - I ask some impressive people just 1 question</li>
                <li>[Udemy course] <a href="https://t.co/1W26wp7ykg?amp=1">A beginner's guide to figma</a> - New to Figma, definitely check it out!</li>
                <li>[Poetry publication] <a href="https://medium.com/millennial-poets">Millennialpoets</a> - Are you a millennial, do you write or read poetry? Join us</li>
                <li>[Iwrite] <a href="https://iwrite.today/">Iwrite</a> - I'm working on a website where anyone can take writing challenges. Join the waitlist</li>
                <li>[A collection of short stories] <a href="">Love in Berlin</a> - I'm currently working on a collection of short stories about love and relationships in Berlin. Check out one of the stories.</li>
            </ul>
        </div> -->

        <!-- <div>
            <h2>Some writings elsewhere</h2>
            <ul>
                <li>[Fiction] <a href="https://medium.com/@busayomi/birds-in-flight-d740aa167a1">Birds in flight</a></li>
                <li>[Poetry] <a href="https://medium.com/millennial-poets/the-poem-e14377693eeb">The poem</a></li>
                <li>[Essay] <a href="https://medium.com/millennial-poets/why-poetry-matters-57c86a072c35">Why poetry matters</a></li>
                <li>[Musing] <a href="https://medium.com/millennial-poets/o-me-o-life-1c64df6b702a">O Me! O life!</a></li>
                 <li>[Musing/ Article] <a href="https://medium.com/@busayomi/revamping-yourself-222229ebfae6">Revamping yourself</a></li>
                <li>[Article] <a href="https://medium.com/@busayomi/the-fascinating-notion-of-speed-learning-4343483451e3">The Fascinating Notion of Speed Learning</a></li>
                <li>[Design article] <a href="https://medium.com/@busayomi/making-accessibility-the-default-f8a9f1d8e259">Making Accessibility the Default</a></li>
                <li>[Design article] <a href="https://uxdesign.cc/how-visually-impaired-people-navigate-the-web-7f9eab9d9c37">How visually impaired people navigate the web</a></li>
                <li>[Design article] <a href="https://uxdesign.cc/how-to-efficiently-use-figma-community-resources-d94c909d3a69">How to efficiently use Figma community resources</a></li>
                <li>[Design article] <a href="https://uxdesign.cc/how-to-navigate-your-entry-level-ux-job-baa42c76d0f0">How to navigate your entry-level UX job</a></li>
                <li>[Dev article] <a href="https://medium.com/@busayomi/before-and-after-pseudo-elements-3fcc7928626d">Before and After Pseudo Elements</a></li>
                <li>[Dev article] <a href="https://medium.com/@busayomi/why-you-should-write-semantic-html-bd389ffda9f4">Why you should write semantic HTML</a></li>
            </ul>

        </div> -->
        
    </Layout>
</template>

export default {
  metaInfo: {
    title: 'Home'
  }
}

<style lang="scss">
.post-title {
  padding: calc(var(--space) / 2) 0 calc(var(--space) / 2);
  text-align: center;
}
.post {
  &__header {
    width: calc(100% + var(--space) * 2);
    margin-left: calc(var(--space) * -1);
    margin-top: calc(var(--space) * -1);
    margin-bottom: calc(var(--space) / 2);
    overflow: hidden;
    border-radius: var(--radius) var(--radius) 0 0;
    img {
      width: 100%;
    }
    &:empty {
      display: none;
    }
  }
  &__content {
    h2:first-child {
      margin-top: 0;
    }
    p:first-of-type {
      font-size: 1.2em;
      color: var(--title-color);
    }
    img {
      width: calc(100% + var(--space) * 2);
      margin-left: calc(var(--space) * -1);
      display: block;
      max-width: none;
    }
  }
}
.post-comments {
  padding: calc(var(--space) / 2);
  &:empty {
    display: none;
  }
}
.post-author {
  margin-top: calc(var(--space) / 2);
}
a {
	color: #FDB310 !important;
}
.intro-box {
  display: flex;
  flex-wrap: wrap;
}

.profile-header {
  display: block;
  width: 50%;
  margin-left: auto;
  margin-right: auto;
  margin-bottom: 50px;
}

.profile-img{
  width: 12em;
  height: 12em;
  border-radius: 50%;
}

.profile-header h2 {
  margin: 0;
}

</style>

