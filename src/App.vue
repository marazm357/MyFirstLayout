<template>
  <div class="container">
    <div class="header">
      <div class="logo">
        <img src="images\logo1.png" alt="logo" height="56px" />
      </div>
      <div>
        <div class="tema">
          <button class="btmTema">
            <img src="images/moon.svg" alt="moon" width="20px" />
          </button>
        </div>
      </div>
    </div>

    <div class="nav-bar">
      <div class="nav-cards">
        <nav class="nav-card">
          <div class="homeCard">
            <router-link class="home-card" to="/">
              <img src="images\home.png" alt="home" />
              <span>Home</span>
            </router-link>
          </div>
          <div class="resumeCard">
            <router-link class="resume-card" to="/about">
              <img src="images\resume.png" alt="home" />
              <span>Resume</span>
            </router-link>
          </div>
          <div class="workCard">
            <router-link class="work-card" to="/work">
              <img src="images\work.png" alt="home" />
              <span>Work</span>
            </router-link>
          </div>
          <div class="contactCard">
            <router-link class="contact-card" to="/">
              <img src="images\contact.png" alt="home" />
              <span>Contact</span>
            </router-link>
          </div>
        </nav>
      </div>
    </div>
    <div class="content">
      <div class="profileCard">
        <div class="profileImage">
          <img src="images/gig.jpg" height="200px" width="200px" alt="giga" />
        </div>
        <div class="Names">
          <h3>GigaChad</h3>
          <span>Front-end Developer</span>
        </div>
        <div class="social">
          <div class="soc">
            <a href="https://vk.com/sber">
              <img src="images/vk.png" alt="logo" width="30px" />
            </a>
          </div>
          <div class="soc">
            <a href=""
              ><img src="images/telega.png" alt="logo" width="30px"
            /></a>
          </div>
          <div class="soc">
            <a href="mailto:sberbank@sberbank.ru"
              ><img src="images/email.png" alt="logo" width="30px"
            /></a>
          </div>
          <div class="soc">
            <a href="github"
              ><img src="images/git.png" alt="logo" width="30px" />
            </a>
          </div>
        </div>
        <div class="contact">
          <div class="phoneCard">
            <div class="phoneIcon">
              <img src="images/phone.svg" alt="phone" />
            </div>
            <div class="phoneInfo">
              <span>Phone</span>
              <a href="">+2573477835</a>
            </div>
          </div>
          <div class="contactHr"></div>
          <div class="emailCard">
            <div class="emailIcon">
              <img src="images/email.svg" alt="email" />
            </div>
            <div class="emailInfo">
              <span>Email</span>
              <a href="">help@mail.oxfordalumni.org</a>
            </div>
          </div>
          <div class="contactHr"></div>
          <div class="locationCard">
            <div class="locationIcon">
              <img src="images/location.svg" alt="location" />
            </div>
            <div class="locationInfo">
              <span>Location</span>
              <a
                href="https://yandex.ru/maps/org/sberbank/145424245397/?ll=38.972169%2C45.022119&z=17.52"
                >Moscow, Russia, Sberbank</a
              >
            </div>
          </div>
          <div class="contactHr"></div>
          <div class="downloadBtn">
            <img src="images/download.svg" alt="down" />
            <a href="">Download Resume</a>
          </div>
        </div>
      </div>
      <div class="aboutSection">
        <router-view></router-view>
      </div>
    </div>
  </div>
</template>

<script>
import HomeViewVue from "./components/HomeView.vue";
import ResumeView from "./components/ResumeView.vue";
import WorkView from "./components/WorkView.vue";

export default {
  HomeViewVue,
  ResumeView,
  WorkView,
};
</script>

<style lang="scss">
#app {
  font-family: "Raleway", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
body {
  background-color: #f2f5f9;
}
.container {
  margin: 0;
  max-width: 1440px;
  height: 1024px;

  .header {
    display: flex;
    max-width: 1240px;
    height: 104px;
    padding: 44px 0px;
    justify-content: space-between;
    align-items: center;
    flex-shrink: 0;
    margin: 18px 100px 0px;
  }
  .btmTema {
    display: flex;
    width: 56px;
    height: 56px;
    padding: 10px;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 10px;
    flex-shrink: 0;
    border-radius: 50px;
    box-shadow: 0px 0px 4px 0px rgba(0, 0, 0, 0.25);
    border: 1px;
    background: #ebf2fa;
  }
  .nav-bar {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-end;
    gap: 10px;
    margin: 0px 100px;

    .nav-cards {
      width: 503px;
      height: 100px;
      border-radius: 20px;
      background: #f2f7fc;
    }
    .nav-card {
      display: flex;
      justify-content: center;
      align-items: center;
      gap: 40px;
      box-shadow: 0px 0px 4px 0px rgba(0, 0, 0, 0.25);
      padding: 10px 0;
      border-radius: 20px;
      background-color: #f2f7fc;
    }
  }
  .homeCard {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    width: 80px;
    height: 80px;
    background: linear-gradient(80deg, #ff9c1a 5%, #e80505 100%);
    border-radius: 20px;
  }
  .resumeCard {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    width: 80px;
    height: 80px;
    background: #e1e8ef;
    border-radius: 20px;
  }
  .workCard {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    width: 80px;
    height: 80px;
    background: #e1e8ef;
    border-radius: 20px;
  }
  .contactCard {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    width: 80px;
    height: 80px;
    background: #e1e8ef;
    border-radius: 20px;
  }
  .home-card {
    display: flex;
    flex-direction: column;
    align-items: center;
    color: #fff;
    font-size: 12px;
    font-style: normal;
    font-weight: 600;
    line-height: 20px; /* 166.667% */
    text-decoration: none;
  }
  .home-card img {
    width: 24px;
    height: 24px;
  }
  .resume-card {
    display: flex;
    flex-direction: column;
    align-items: center;
    color: #000000;
    font-size: 12px;
    font-style: normal;
    font-weight: 600;
    line-height: 20px; /* 166.667% */
    text-decoration: none;
  }
  .work-card {
    display: flex;
    flex-direction: column;
    align-items: center;
    color: #000000;
    font-size: 12px;
    font-style: normal;
    font-weight: 600;
    line-height: 20px; /* 166.667% */
    text-decoration: none;
  }
  .contact-card {
    display: flex;
    flex-direction: column;
    align-items: center;
    color: #000000;
    font-size: 12px;
    font-style: normal;
    font-weight: 600;
    line-height: 20px; /* 166.667% */
    text-decoration: none;
  }
  .content {
    display: flex;
    margin: 10px 100px 0 100px;
    gap: 20px;
  }
  .profileCard {
    background-color: #fff;
    width: 400px;
    height: 700px;
    display: flex;
    flex-direction: column;
    align-items: center;
    flex-shrink: 0;
    border-radius: 20px;
  }
  .profileImage {
    max-width: 200px;
    max-height: 200px;
    position: relative;
    bottom: 100px;
    img {
      border-radius: 20px;
      box-shadow: 0px 0px 4px 0px rgba(0, 0, 0, 0.25);
    }
  }
  .aboutSection {
    width: 820px;
    height: 700px;
    background-color: yellow;
  }
  .Names {
    position: relative;
    bottom: 100px;
    display: flex;
    flex-direction: column;
    align-items: center;

    span {
      color: rgba(11, 9, 9, 0.5);
      font-size: 16px;
      font-style: normal;
      font-weight: 500;
      line-height: 40px; /* 250% */
      margin: 0;
      padding: 0;
    }
    h3 {
      margin: 14px 0 4px 0;
      color: #0b0909;
      font-family: Raleway;
      font-size: 28.42px;
      font-style: normal;
      font-weight: 700;
      line-height: 35.525px; /* 125% */
    }
  }
  .social {
    position: relative;
    width: 180px;
    display: flex;
    justify-content: space-around;
    gap: 10px;
    bottom: 90px;
  }
  .soc {
    padding: 15px;
    height: 30px;
    background-color: #f2f7fc;
    border-radius: 25%;
  }
  .aboutSection {
    max-width: 820px;
    max-height: 700px;
    border-radius: 20px;
    background-color: #fff;
  }
  .phoneCard {
    display: flex;
    justify-content: center;
    gap: 26px;
    .phoneIcon {
      display: flex;
    }
  }
  .phoneInfo {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    color: rgba(26, 16, 3, 0.5);
    font-size: 14px;
    font-style: normal;
    font-weight: 600;
    gap: 3px;
    a {
      text-decoration: none;
      color: #000;
      font-family: Raleway;
      font-size: 14px;
      font-style: normal;
      font-weight: 600;
    }
  }
  .emailCard {
    display: flex;
    justify-content: center;
    gap: 26px;
    .emailIcon {
      display: flex;
    }
  }
  .emailInfo {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    color: rgba(26, 16, 3, 0.5);
    font-size: 14px;
    font-style: normal;
    font-weight: 600;
    gap: 3px;
    a {
      text-decoration: none;
      color: #000;
      font-family: Raleway;
      font-size: 14px;
      font-style: normal;
      font-weight: 600;
    }
  }
  .contact {
    position: relative;
    bottom: 60px;
    background-color: #f2f5f9;
    border-radius: 20px;
    padding: 30px 30px 40px 30px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    gap: 20px;
    .downloadBtn {
      position: relative;
      left: 20px;
      background: linear-gradient(80deg, #ff9c1a 5%, #e80505 100%);
      display: flex;
      justify-content: center;
      align-items: center;
      gap: 10px;
      padding: 10px 20px;
      border-radius: 20px;
      a {
        text-decoration: none;
        color: #f2f7fc;
      }
    }
  }
  .locationCard {
    display: flex;
    justify-content: center;
    gap: 26px;
    .locationIcon {
      display: flex;
    }
  }
  .locationInfo {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    color: rgba(26, 16, 3, 0.5);
    font-size: 14px;
    font-style: normal;
    font-weight: 600;
    gap: 3px;
    a {
      text-decoration: none;
      color: #000;
      font-family: Raleway;
      font-size: 14px;
      font-style: normal;
      font-weight: 600;
    }
  }
  .contactHr {
    width: 256px;
    height: 1px;
    background: #e3e3e3;
  }
}
</style>
