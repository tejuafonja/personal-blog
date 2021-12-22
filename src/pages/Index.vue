<template>
  <Layout class="content-box" :show-logo="false" :show-nav="true">
    <h1>Tẹjúmádé Àfọ̀njá</h1>
    <div class="profile-header">
      <div class="profile-header__img">
          <g-image
          src="~/assets/images/about-img.jpg"
          class="profile-img"
        ></g-image>
        
      </div>
        <div class="profile-header__intro">
          I am the co-founder of 
          <a href="http://www.aisaturdayslagos.com/" target="_blank">AI Saturdays Lagos</a>, 
          an artificial intelligence community in Lagos, Nigeria. 
          I work at CISPA as a research assistant under the supervision of 
          <a href="https://cispa.saarland/group/fritz/" target="_blank">Prof. Mario Fritz</a>  
          where I conduct research on learning generative models 
          for tabular data. I lead the <a href="https://sautiproject.com" target="_blank">Sauti Project</a>, 
          work focused on improving accented speech research in Africa. 
          <!-- and conducted under 
          <a href="https:tri-ai.org" target="_blank"> TRI-AI </a>, 
          a non-profit organization I co-founded. -->
        </div>
    </div>

    <div class="more-details">
        <div>
          During the summer of 2020, I had the opportunity to intern remotely with
          <a href="https://www.papernot.fr/" target="_blank"
            >Prof. Nicolas Papernot</a
          >
          at the University of Toronto and Vector Institute where I investigated
          the security of speaker classification models, specifically, I worked
          on generative model extraction of speaker classification models.
        </div>

        <div>
          In 2018, I co-founded
          <a href="http://www.aisaturdayslagos.com/" target="_blank">AI Saturdays Lagos</a>, 
          an artificial intelligence community based in Lagos, Nigeria, 
          a completely volunteer-driven initiative 
          where we offer free classes on Data Science, Machine Learning and Deep
          Learning for about 16 weeks (classes are on Saturdays) through
          structured learning groups. We recently concluded our  
          <a href="https://github.com/AISaturdaysLagos/cohort7_structure" target="_blank">7th cohort</a>, 
          focused on Data Science and Machine Learning.
          Since the onset of the pandemic, we now teach our classes virtually.
        </div>

        <div>
          For the past two years, I have 
          co-organized the Mechanism Design for Social Good development working group(<a
            href="https://www.md4sg.com/workinggroups/dev.html"
            target="_blank"
            >MD4SG-Dev</a
          >). I have also co-organized Machine Learning for the Developing World (<a
            href="https://sites.google.com/view/ml4d/home?authuser=0"
            target="_blank"
            >ML4D</a
          >) NeurIPS workshop for three consecutive years, where I served as the lead organizer in 2020 and the
          chair of the steering committee in 2021.
        </div>

        <div>
          You can stay in touch with me via
          <a href="https://linkedin.com/in/tejumadeafonja">LinkedIn</a> or 
          <a href="https://twitter.com/tejuafonja">Twitter</a>. 
          You can also contact me via <a mail-to="teju.afonja@aisaturdayslagos.com" target="_blank">email</a>.
        </div>
      
        <div>
          I write on <g-link to="/xhirot">Xhirot</g-link>, 
          <a href="https://medium.com/@tejuafonja" target="_blank">my Medium page</a>, and
          <a href="https://medium.com/ai-saturdays-lagos-articles" target="_blank">AISaturdaysLagos Medium page</a>
        </div>

      </div>
  </Layout>
</template>

export default {
  metaInfo: {
    title: 'Home'
  }
}


<style lang="scss">
a {
  color: #fdb310 !important;
}

.content-box h1 {
  margin-top: 1rem;
  margin-bottom: 2rem;
  text-align: center;
}
.more-details {
  display: flex;
  flex-wrap: wrap;
  margin-top: 1.5rem;
  & div {
    margin-bottom: 1.5rem;
    text-align: justify;
  }
}
.profile-header {
  display: flex;
  width: 100%;

&__img {
  display: block;
  width: 60%;
  margin-right: 1rem;
  }

&__intro{
  width: 100%;
  text-align: justify;
  }
}

.profile-img {
  width: 12em;
  height: 12em;
}
@media screen and (max-width: 650px) {
  .profile-header {
  display: flex;
  flex-direction: column;
  }

  .profile-header {

  &__img {
  width: 100%;
  text-align: center;

  }

  &__intro {
    margin-top: 1.5rem;
    }
  
  }

}

</style>



