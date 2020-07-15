<template>
  <body>

    <div id="nav-scroller" ref="content">
      <div class="title" id="home">
        <div>
          <h1>Hi, I am Shubham Pasari.</h1>
          <h3>And this is my Interactive Resume!</h3>
        </div>
      </div>

      <div class="temporary">
      </div>

      <nav id="nav-bar">
        <div class="navbar-header">
          <div id="navbar-button">
            <span class="icon-navbar" @click="showOrHideNavbar" :class="[navbarOpen ? 'open-navbar' : 'closed-navbar']"></span>
          </div>
        </div>
        <div :class="[navbarOpen ? 'show-navbar' : 'collapse-navbar']">
          <ul>
            <li :class="{ 'current' : (activeClass == 'about') }"><a href="#about" v-smooth-scroll><p>About</p></a></li>
            <li :class="{ 'current' : (activeClass == 'education') }"><a href="#education" v-smooth-scroll><p>Education</p></a></li>
            <li :class="{ 'current' : (activeClass == 'work') }"><a href="#work" v-smooth-scroll><p>Work</p></a></li>
            <li :class="{ 'current' : (activeClass == 'skills') }"><a href="#skills" v-smooth-scroll><p>Skills</p></a></li>
            <li :class="{ 'current' : (activeClass == 'projects') }"><a href="#projects" v-smooth-scroll><p>Projects</p></a></li>
            <li :class="{ 'current' : (activeClass == 'contact') }"><a href="#contact" v-smooth-scroll><p>Contact</p></a></li>
          </ul>
        </div>
      </nav>

      <div class="about" id="about">
        <h1>Profile</h1>

        <h4>I'm an Android and Web Developer</h4>

        <hr>

        <div class="row">
          <div class="four columns about-me">
            <h2>About Me</h2>
            <p>
              I am an Engineering Student pursuing Mathematics and Computing from Delhi Technological University(Formerly Delhi College of Engineering). I have exprience in Android Development, Web development using Vue and Machine Learning. I love structure and quality of the front-end and spend time fixing the little details on my projects. I like to work in groups as it helps me to learn a lot about new stuffs too.
            </p>

          </div>
          <div class="three columns profile-picture">
            <img class="picture" src="../assets/shubham_pasari.jpg" alt="Shubham Pasari" width="180" height="180">
          </div>
          <div class="five columns details">
            <h3>Name:</h3>
            <p>Shubham Pasari</p>
            <h3>Age:</h3>
            <p>23</p>
            <h3>Location</h3>
            <p>New Delhi</p>
            <div class="button" id="download-resume">
              <a href="https://drive.google.com/file/d/10ytRBZwdr4_OXxdDC3uWRN1HhYS6-g3p/view?usp=sharing" target="_blank">
                <p>Download Resume</p>
              </a>
            </div>
          </div>
        </div>
      </div>

      <div class="education-container">

        <div class="education" id="education">
          <h1>Education</h1>
          <hr>
          <div class="row">
            <div class="three columns institution">
              <h3><span>Delhi Technological University</span></h3>
              <h5>2016-2020</h5>
            </div>

            <div class="seven columns institution-description">
              <h4>Major: Mathematics and Computing</h4>
              <h5>CGPA: 8.29/10</h5>
              <p>This course consists of subjects related to Pure Mathematics, Applied Mathematics and Computer Science. Statistics, Probability, Real Number, Linear Algebra, Scientific Computation, ADA, DBMS, Operating Systems etc., are some of the important subject taught in this course.</p>
            </div>

            <div class="three columns institution" style="margin-top: 30px;">
              <h3><span>Hope Hall Foundation School</span></h3>
              <h5>2013-2015</h5>
            </div>

            <div class="seven columns institution-description" style="margin-top: 30px">
              <h4>Senior Secondary School in Science</h4>
              <h5>Percentage: 92.4</h5>
              <p>This course consists of the subjects Maths, Physics, Chemistry, English and Physical Education.</p>
            </div>
            <div class="three columns institution" style="margin-top: 30px;">
              <h3><span>Delhi Public School</span></h3>
              <h5>2006-2013</h5>
            </div>
            <div class="seven columns institution-description" style="margin-top: 30px">
              <h4>Secondary School in Science</h4>
              <h5>CGPA: 10/10</h5>
              <p>This course consists of the subjects Maths, Physics, Chemistry, English and Physical Education.</p>
            </div>
          </div>
        </div>
      </div>

      <div class="work" id="work">
        <h1>Work Experience</h1>
        <hr>
        <div class="row">
          <div class="three columns institution">
            <h3><span>Pudle</span></h3>
            <h5>Gurugram</h5>
            <h5>May 2019 - July 2019</h5>
          </div>

          <div class="seven columns institution-description">
            <h4>Software Developer Intern</h4>
            <p>Worked on a project to design and develop the Website of the product from scratch using Vue.js, Firebase, Bootstrap Vue and Mapbox along with Various other Places API, Email API, Google Analytics and SMS API</p>
          </div>

          <div class="three columns institution" style="margin-top: 30px;">
            <h3><span>JUSCO</span></h3>
            <h5>Jamshedpur</h5>
            <h5>June 2018 - July 2018</h5>
          </div>

          <div class="seven columns institution-description" style="margin-top: 30px;">
            <h4>Software Developer Intern</h4>
            <p>Worked on a project to create a system to keep track of various re- sources of the company and Keep track of their Servicing. It also included a Email-Reminder System to remind the person for the ser- vicing a few days before the due date. It was developed using Python and MongoDB</p>
          </div>
        </div>

      </div>

      <div class="skills-container">

        <div class="skills" id="skills">
          <h1>Skills</h1>
          <hr>

          <div class="row skills-row">

            <div class="six columns skills-column">
                <ul class="no-bullets">
                  <li class="list-view">
                    <span class="skill-name">Java</span>
                    <span class="rating">
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star">★</span>
                    </span>
                  </li>
                  <li class="list-view">
                    <span class="skill-name">Python</span>
                    <span class="rating">
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star">★</span>
                    </span>
                  </li>
                  <li class="list-view">
                    <span class="skill-name">Javascript</span>
                    <span class="rating">
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star">★</span>
                    </span>
                  </li>
                  <li class="list-view">
                    <span class="skill-name">Android</span>
                    <span class="rating">
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star">★</span>
                    </span>
                  </li>
                  <li class="list-view">
                    <span class="skill-name">Vue.js</span>
                    <span class="rating">
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star">★</span>
                    </span>
                  </li>
                  <li class="list-view">
                    <span class="skill-name">OOPS</span>
                    <span class="rating">
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star">★</span>
                    </span>
                  </li>
                  <li class="list-view">
                    <span class="skill-name">GIT</span>
                    <span class="rating">
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star">★</span>
                      <span class="star">★</span>
                    </span>
                  </li>
                  <li class="list-view">
                    <span class="skill-name">XML</span>
                    <span class="rating">
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star">★</span>
                      <span class="star">★</span>
                    </span>
                  </li>
                  <li class="list-view">
                    <span class="skill-name">C++</span>
                    <span class="rating">
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star">★</span>
                      <span class="star">★</span>
                    </span>
                  </li>
                </ul>
            </div>
            <div class="six columns skills-column">
                <ul class="no-bullets">
                  <li class="list-view">
                    <span class="skill-name">HTML(5)</span>
                    <span class="rating">
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star">★</span>
                      <span class="star">★</span>
                    </span>
                  </li>
                  <li class="list-view">
                    <span class="skill-name">CSS(3)</span>
                    <span class="rating">
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star">★</span>
                      <span class="star">★</span>
                    </span>
                  </li>
                  <li class="list-view">
                    <span class="skill-name">MySQL</span>
                    <span class="rating">
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star">★</span>
                      <span class="star">★</span>
                    </span>
                  </li>
                  <li class="list-view">
                    <span class="skill-name">Firebase</span>
                    <span class="rating">
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star">★</span>
                      <span class="star">★</span>
                    </span>
                  </li>
                  <li class="list-view">
                    <span class="skill-name">PostgreSQL</span>
                    <span class="rating">
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star">★</span>
                      <span class="star">★</span>
                    </span>
                  </li>
                  <li class="list-view">
                    <span class="skill-name">Operating Systems</span>
                    <span class="rating">
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star">★</span>
                      <span class="star">★</span>
                    </span>
                  </li>
                  <li class="list-view">
                    <span class="skill-name">Machine Learning</span>
                    <span class="rating">
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star">★</span>
                      <span class="star">★</span>
                    </span>
                  </li>
                  <li class="list-view">
                    <span class="skill-name">Deep Learning</span>
                    <span class="rating">
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star">★</span>
                      <span class="star">★</span>
                      <span class="star">★</span>
                    </span>
                  </li>
                  <li class="list-view">
                    <span class="skill-name">C</span>
                    <span class="rating">
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star">★</span>
                      <span class="star">★</span>
                      <span class="star">★</span>
                    </span>
                  </li>
                </ul>
            </div>
          </div>

          <div class="website-code-link">
            <p class="github-text">This project is built using Vue.js and Bootstrap Vue. Interested to see the source code?</p>
            <div class="button github-source-code">
              <a href="" target="_blank">
                <p>See Project on Github</p>
              </a>
            </div>
          </div>

          <hr>

          <h2 class="title-languages">Languages</h2>
          <div class="row skills-row languages-row">

            <div class="six columns skills-column">
                <ul class="no-bullets">
                  <li class="list-view">
                    <span class="skill-name">Hindi (Mother tongue)</span>
                    <span class="rating">
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                    </span>
                  </li>
                  <li class="list-view">
                    <span class="skill-name">English (Daily use)</span>
                    <span class="rating">
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                    </span>
                  </li>
                </ul>
            </div>
            <div class="six columns skills-column">
                <ul class="no-bullets">
                  <li class="list-view">
                    <span class="skill-name">German (Beginner)</span>
                    <span class="rating">
                      <span class="star filled">★</span>
                      <span class="star filled">★</span>
                      <span class="star">★</span>
                      <span class="star">★</span>
                      <span class="star">★</span>
                    </span>
                  </li>
                </ul>
            </div>
          </div>

        </div>

      </div>

      <div class="projects" id="projects">
        <h1>Projects</h1>
        <h3>"There are many things that, if I have to relive, maybe I will do it another way. But I would not like to look back and think what I have not been able to do"</h3>
        <h3>-Ratan Tata</h3>
        <hr>

        <div class="row projects-row">
          <div class="four columns">
            <div class="project-container">
              <div class="project-object">
                <img class="project-image" src="../assets/news_app.jpg" alt="News App">
                <div class="on-hover">
                  <a href="https://github.com/Shubh0501/News_App" class="project-link" target="_blank"></a>
                  <div class="project-description-animation">
                    <h4>NewsApp</h4>
                    <p>Android Project to show latest news in India</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="four columns">
            <div class="project-container">
              <div class="project-object">
                <img class="project-image" src="../assets/photoapp.png" alt="">
                <div class="on-hover">
                  <a href="https://github.com/Shubh0501/PhotoApp" class="project-link" target="_blank"></a>
                  <div class="project-description-animation">
                    <h4>PhotoApp</h4>
                    <p>Android project to save photos securely in local storage</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="four columns">
            <div class="project-container">
              <div class="project-object">
                <img class="project-image" src="../assets/myshopping.png" alt="">
                <div class="on-hover">
                  <a href="https://github.com/Shubh0501/MyShopping" class="project-link" target="_blank"></a>
                  <div class="project-description-animation">
                    <h4>MyShopping</h4>
                    <p>Android project to let users track their shopping</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="four columns">
            <div class="project-container">
              <div class="project-object">
                <img class="project-image" src="../assets/asset_management_system.jpg" alt="">
                <div class="on-hover">
                  <a href="https://github.com/Shubh0501/Assets-Management-System" class="project-link" target="_blank"></a>
                  <div class="project-description-animation">
                    <h4>Assets Management System</h4>
                    <p>Python project to track the assets of an organisation</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="four columns">
            <div class="project-container">
              <div class="project-object">
                <img class="project-image" src="../assets/medic.jpg" alt="">
                <div class="on-hover">
                  <a href="https://github.com/Shubh0501/Medic" class="project-link" target="_blank"></a>
                  <div class="project-description-animation">
                    <h4>Medic</h4>
                    <p>Python project to predict the most probable disease based on the symptoms</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="four columns">
            <div class="project-container">
              <div class="project-object">
                <img class="project-image" src="../assets/language_model.jpg" alt="">
                <div class="on-hover">
                  <a href="https://drive.google.com/file/d/13LGt9FD1WnEy314_8dimhHhyZU8W1tOZ/view?usp=sharing" class="project-link" target="_blank"></a>
                  <div class="project-description-animation">
                    <h4>Language Modelling of Code Switched Data</h4>
                    <p>Research work to classify Humorous data using Language Model</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="contact-container">
        <div class="contact" id="contact">
          <h1>Contact Information</h1>
          <h3>Your work is going to fill a large part of your life, and the only way to be truly satisfied is to do what you believe is great work. And the only way to do great work is to love what you do. If you haven't found it yet, keep looking. Don't settle. As with all matters of the heart, you'll know when you find it.</h3>
          <h3>-Steve Jobs</h3>
          <hr>

          <div class="row contact-information">
            <div class="six columns contact-column">
              <ul class="contact-list">
                <li class="contact-item">
                  <a href="https://www.facebook.com/shubham.pasari.05/" target="_blank" class="social-link">
                    <span class="icon icon-facebook"></span>
                    https://www.facebook.com/shubham.pasari.05/
                  </a>
                </li>
                <li class="contact-item">
                  <a href="https://www.linkedin.com/in/shubham-pasari" target="_blank"  class="social-link">
                    <span class="icon icon-linkedin"></span>
                    https://www.linkedin.com/in/shubham-pasari
                  </a>
                </li>
              </ul>
            </div>
            <div class="six columns contact-column">
              <ul class="contact-list">
                <li class="contact-item">
                  <a href="https://www.instagram.com/shubham_pasari/" target="_blank"  class="social-link">
                    <span class="icon icon-instagram"></span>
                    https://www.instagram.com/shubham_pasari/
                  </a>
                </li>
                <li class="contact-item">
                  <a href="mailto:shubham050197@gmail.com" target="_blank"  class="social-link">
                    <span class="icon icon-gmail"></span>
                    shubham050197@gmail.com
                  </a>
                </li>
              </ul>
            </div>
          </div>

          <hr>

        </div>
      </div>
    </div>
  </body>
</template>

<script>
export default {
  name: 'Main',
  created () {
    window.addEventListener('scroll', this.handleScroll, { passive: true })
  },
  destroyed () {
    window.removeEventListener('scroll', this.handleScroll)
  },
  data () {
    return {
      activeClass: '',
      navbarOpen: false
    }
  },
  methods: {
    showOrHideNavbar () {
      this.navbarOpen = !this.navbarOpen
    },

    onActivate (target) {
      this.activeClass = target
      console.log(document.title)
    },

    handleScroll (event) {
      var about = document.getElementById('about').offsetTop
      var education = document.getElementById('education').offsetTop
      var work = document.getElementById('work').offsetTop
      var skills = document.getElementById('skills').offsetTop
      var projects = document.getElementById('projects').offsetTop
      var contact = document.getElementById('contact').offsetTop
      var current = document.documentElement.scrollTop
      var windowHeight = document.documentElement.scrollHeight
      if (document.documentElement.scrollTop >= 0) {
        current = document.documentElement.scrollTop
        windowHeight = document.documentElement.scrollHeight
      } else if (document.body.scrollTop >= 0) {
        current = document.body.scrollTop
        windowHeight = document.body.scrollHeight
      }
      if (current < about) {
        this.activeClass = ''
      } else if (current < education) {
        this.activeClass = 'about'
      } else if (current < work) {
        this.activeClass = 'education'
      } else if (current < skills) {
        this.activeClass = 'work'
      } else if (current < projects) {
        this.activeClass = 'skills'
      } else if (current < contact && (window.innerHeight + window.scrollY) < windowHeight) {
        this.activeClass = 'projects'
      } else {
        this.activeClass = 'contact'
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

  body {
    margin: 0;
    padding: 0;
    border: 0;
    background: transparent;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  }

  hr {
    margin-left: 20%;
    margin-right: 20%;
  }

  * {
    display: block;
    overflow: hidden;
  }

  div.title {
    height: 100vh;
    width: 100vw;
    top: 0;
    left: 0;
    position: absolute;
    background-color: steelblue;
    text-align: center;
    align-items: center;
    display: flex;
  }

  div.temporary {
    z-index: -100;
    background-color: white;
    height: 100vh;
    width: 100vw;
    position: relative;
  }

  .title h1 {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    color: white;
    text-align: center;
    font-weight: bolder;
    font-size: 50px;
    width: 100vw;
  }

  .title h3 {
    color: white;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    font-weight: bold;
    font-size: 25px;
    text-align: center;
  }

  .about {
    background-color: white;
    text-align: center;
    position: relative;
  }

  .about h1, .education h1, .work h1, .skills h1, .projects h1 {
    margin: 0;
    padding-top: 30px;
    align-items: center;
    font-size: 50px;
    color: darkcyan;
    font-weight: 500;
  }

  .about h4 {
    color: slategray;
    font-size: 20px;
    font-weight: 400;
    margin: 10px;
  }

  .about-me h2 {
    color: darkcyan;
    font-weight: 400;
    font-size: 30px;
    text-align: center;
  }

  .about-me p {
    color: darkslategray;
    padding: 10px 30px 10px 30px;
    text-align: justify;
  }

  .profile-picture {
    justify-content: center;
    display: flex;
  }

  .picture {
    width: 100%;
    max-width: 300px;
    border-radius: 50%;
    height: auto;
  }

  .details {
    margin-top: 30px;
  }

  .details h3 {
    color: darkslategray;
    font-weight: 700;
    font-size: 16px;
  }

  .details p {
    color: darkslategray;
    margin: 0;
    font-style: normal;
    text-decoration: none;
  }

  .button {
    margin-top: 30px;
    background-color: darkcyan;
    width: fit-content;
    border-radius: 12px;
    display: inline-block;
    justify-content: center;
  }

  #download-resume a {
    text-decoration: none;
    justify-content: center;
  }

  #download-resume p {
    color: white;
    padding: 20px;
  }

  #download-resume > a:hover {
    text-decoration: underline;
    text-decoration-color: white;
  }

  .education-container, .skills-container {
    margin-top: 40px;
    background-color: #ede6e6;
    color: darkslategray;
  }

  .row {
    margin: 10px 30px 10px 30px;
  }

  .institution {
    margin: 20px 20px 30px 0;
  }

  .institution-description h5{
    margin-bottom: 30px !important;
  }

  .work {
    color: darkslategray;
    padding-bottom: 50px;
  }

  .education h1, .work h1, .skills h1, .projects h1, .contact h1 {
    text-align: center;
  }

  .education > .row > .institution h5, .work > .row > .institution h5 {
    margin: 0;
    font-weight: 300;
  }

  .education > .row > .institution-description h4, .work > .row > .institution-description h4 {
    font-size: 16px;
    margin-bottom: 0;
    font-weight: 500;
  }

  .education > .row > .institution-description h5{
    font-size: 14px;
    margin: 0;
    margin-top: 5px;
    font-weight: 400;
  }

  .education > .row > .institution-description p{
    font-size: 15px;
    margin: 0;
    word-spacing: 2px;
    margin-top: 8px;
    line-height: 1.6;
  }

  .work > .row > .institution-description p{
    word-spacing: 2px;
    line-height: 1.6;
    margin: 0;
    margin-top: 8px;
    word-wrap: break-word;
    font-size: 15px;
  }

  .skills-row {
    margin: 0;
    display: block !important;
    position: relative;
    overflow: hidden;
  }

  .skill-name {
    text-align: left;
    display: inline-block;
    font-size: 15px;
  }

  .no-bullets {
    list-style-type: none;
    margin: 0;
    display: block;
    line-height: 1.6;
    width: 100%;
    padding: 0;
    position: relative;
  }

  .list-view {
    min-height: 30px;
    padding: 3px 0px;
    display: list-item;
    position: relative;
  }

  .rating {
    float: right;
    display: block;
  }

  .star {
    position: relative;
    font-size: 14px;
    font-weight: 500;
    display: inline;
    color: grey;
  }

  .rating > .filled {
    color: darkcyan;
  }

  .website-code-link {
    margin-top: 20px;
    text-align: center;
    position: relative;
  }

  .github-text {
    text-align: center;
    font-size: 12px;
    font-style: italic;
    color: lightslategray;
    margin: 0;
    padding: 0;
    margin-bottom: 10px;
  }

  .github-source-code {
    margin: 0 auto;
    margin-bottom: 15px;
  }

  .github-source-code a {
    text-decoration: none;
  }

  .github-source-code a:hover {
    text-decoration: underline;
    text-decoration-color: white;
  }

  .github-source-code p {
    padding: 10px;
    margin: 0;
    text-align: center;
    color: white;
  }

  .title-languages {
    color: darkcyan;
    font-weight: 500;
    font-size: 30px;
    margin: 0;
    margin-top: 10px;
  }

  .projects h3{
    color: darkslategray;
    font-weight: 400;
    text-align: center;
    margin: 0;
    margin-top: 10px;
  }

  .projects-row {
    text-align: center;
  }

  .project-container {
    overflow: hidden;
    position: relative;
  }

  .project-object {
    display: block;
    cursor: pointer;
    padding: 10px 10px 10px 10px;
  }

  .on-hover {
    position: absolute;
    opacity: 0;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 139, 139, 0.80) repeat;
    transition: opacity 0.35s ease-in-out;
  }

  .project-link {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: 100;
  }

  .projects hr {
    margin-top: 20px;
  }

  .project-object:hover .on-hover{
    opacity: 1;
  }

  .project-image {
    width: 100%;
    height: 100%;
    padding: 20px;
  }

  .project-description-animation {
    position: absolute;
    padding: 20px 30px;
    top: 0;
    left: 0;
  }

  .project-description-animation h4{
    color: white;
    font-size: 20px;
    text-decoration: underline;
    text-transform: uppercase;
  }

  .project-description-animation p {
    color: white;
    font-size: 16px;
  }

  .contact-container {
    background: rgb(31, 33, 31);
  }

  .contact h1 {
    margin: 0;
    padding-top: 30px;
    align-items: center;
    font-size: 50px;
    color: white;
    font-weight: 500;
  }

  .contact h3 {
    color: darkslategray;
    font-weight: 400;
    text-align: center;
    margin: 0;
    margin-top: 10px;
  }

  .contact hr {
    border-color: darkslategray;
    margin-top: 20px;
  }

  .contact-list {
    list-style-type: none;
    line-height: 1.6;
    font-size: 15px;
    text-align: center;
  }

  .contact-information {
    display: block !important;
    overflow: hidden;
  }

  .contact-item a {
    text-decoration: none;
    color: grey;
    unicode-bidi: bidi-override;
    line-height: 32px;
    display: block;
    float: left;
    overflow: hidden;
    margin-bottom: 20px;
    cursor: pointer;
    opacity: 0.7;
  }

  .contact-item a:hover {
    opacity: 1;
  }

  .icon {
    margin-right: 20px;
    background-position: 0px 0px;
    display: inline-block;
    vertical-align: middle;
  }

  .icon-facebook {
    background: url('../assets/facebook.png') no-repeat;
    display: inline-block;
    width: 32px;
    height: 32px;
  }

  .icon-instagram {
    background: url('../assets/instagram.png');
    display: inline-block;
    width: 32px;
    height: 32px;
  }

  .icon-linkedin {
    background: url('../assets/linkedin.png');
    display: inline-block;
    width: 32px;
    height: 32px;
  }

  .icon-gmail {
    background: url('../assets/email.png');
    display: inline-block;
    width: 32px;
    height: 32px;
  }

  @media (max-width: 992px) {
    hr {
      margin-top: 30px;
      margin-bottom: 30px;
    }
    nav {
      font-weight: bold;
      font: 12px;
      width: 100%;
      z-index: 200;
      letter-spacing: 2.5px;
      margin: 0;
      position: fixed;
      top: 0;
    }
    .navbar-header {
      background: black;
      overflow: hidden;
    }
    .icon-navbar {
      float: right;
      display: inline-block;
      width: 100px;
      height: 100px;
      margin-right: 20px;
    }
    .closed-navbar {
      background: url('../assets/navbar-open.png');
    }
    .open-navbar {
      background: url('../assets/navbar-close.png');
    }
    .show-navbar {
      visibility: visible;
    }
    .collapse-navbar {
      visibility: hidden;
      display: none;
    }
    #nav-bar ul {
      width: auto;
      margin-block-start: 0;
      text-align: center;
      background: black;
    }
    #nav-bar li {
      position: relative;
      list-style: none;
    }
    #nav-bar a {
      padding: 10px;
      line-height: 12px;
      display: block;
      text-decoration: none;
      color: white;
    }
    .skills-column {
      margin: 0 30% 0 30%;
    }
    .title-languages {
      text-align: center;
      margin-bottom: 30px;
    }
    .projects h1 {
      margin-bottom: 30px;
    }
    .project-container {
      display: flex;
      justify-content: center;
    }
    .project-object {
      width: 70%;
    }
    .contact-container {
      margin-top: 50px;
      padding-bottom: 100px;
    }
    .contact-container h1 {
      margin-top: 30px;
      margin-bottom: 30px;
    }
    .contact-container h3, .projects h3 {
      margin-left: 30px;
      margin-right: 30px;
    }
    .contact-column {
      text-align: center;
    }
    .contact-list {
      margin: 0;
      display: inline-block;
    }
  }

  @media (min-width: 992px){
    nav {
      font-weight: bold;
      font: 12px;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      width: auto;
      letter-spacing: 2.5px;
      margin: 0;
      z-index: 100;
      position: fixed;
      top: 25%;
      right: 5%;
    }
    .navbar-header {
      visibility: hidden;
    }
    #nav-bar ul {
      width: auto;
      text-align: center;
      background: black;
      padding-inline-start: 0px;
      padding-inline-end: 0px;
    }

    #nav-bar li {
      position: relative;
      list-style: none;
      -webkit-transition: color .2s ease-in-out;
      -moz-transition: color .2s ease-in-out;
      -o-transition: color .2s ease-in-out;
      -ms-transition: color .2s ease-in-out;
      transition: color .2s ease-in-out;
    }

    #nav-bar a {
      padding: 10px;
      line-height: 12px;
      display: inline-block;
      text-decoration: none;
      color: white;
    }

    li.current  {
      background-color: teal !important;
      -webkit-transition: color 0.2s ease-in-out;
      -moz-transition: color 0.2s ease-in-out;
      -o-transition: color 0.2s ease-in-out;
      -ms-transition: color 0.2s ease-in-out;
      transition: color 0.2s ease-in-out;
    }
    * {
      box-sizing: border-box;
    }
    .about, .education, .work, .projects, .contact {
      width: 980px;
      margin: 0 auto;
    }
    .row {
      display: table;
      content: " ";
    }

    .about {
      padding-bottom: 50px;
    }

    .about > .row {
      margin-top: 60px;
    }

    .about > .row > .four {
      padding-left: 50px;
      padding-right: 30px;
      text-align: justify;
      letter-spacing: 1px;
      line-height: 1.6;
    }

    .about > .row > .three {
      padding: 20px;
    }

    .about > .row > .five {
      text-align: left;
      padding-right: 10px;
      padding-left: 40px;
      padding-top: 35px;
    }

    .picture {
      max-width: 140px !important;
    }

    .details {
      float: right !important;
      margin-top: 0;
    }

    .education-container {
      padding-bottom: 50px;
    }

    .education > .row {
      margin-top: 60px;
    }

    .institution {
      margin: 0;
    }

    .institution h3 {
      margin-bottom: 5px;
    }

    .education > .row > .institution-description, .work > .row > .institution-description {
      padding-left: 80px;
    }

    .work > .row {
      margin-top: 60px;
    }

    .work > .row > .institution h5 {
      margin-top: 10px;
    }

    .institution-description h5 {
      margin-bottom: 0 !important;
    }

    .institution-description p {
      text-align: left;
      word-wrap: break-word;
      overflow-wrap: break-word;
    }

    .skills {
      margin: 50px 25% 50px 25%;
    }

    .no-bullets {
      padding-top: 20px;
      padding-bottom: 30px;
      padding-left: 10%;
      padding-right: 10%;
    }

    .skills-column {
      padding-left: 15px;
      padding-right: 15px;
    }

    .languages-row {
      padding-bottom: 30px;
    }

    .contact-container {
      padding-bottom: 200px;
    }

    .row .one {
      width: 8.333333%;
    }
    .row .two {
      width: 16.666667%;
    }
    .row .three {
      width: 25%;
    }
    .row .four {
      width: 33.3333333%;
    }
    .row .five {
      width: 41.66666667%;
    }
    .row .six {
      width: 50%;
    }
    .row .seven {
        width: 58.3333333%;
    }
    .row .eight {
      width: 66.66666667%;
    }
    .row .nine {
      width: 75%;
    }
    .row .ten {
      width: 83.33333333%;
    }
    .row .eleven {
      width: 91.666666667%;
    }
    .row .twelve {
      width: 100%;
    }
    .row .columns {
      float: left;
      position: relative;
    }
  }
</style>
