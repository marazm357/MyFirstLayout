<template>
  <div class="mainInfo">
    <div class="containerHome">
      <div class="headerHome">
        <span>ABOUT ME</span>
        <div class="hrHeader"></div>
      </div>
      <div class="infoHome">
        <p>
          Hello there! I'm thrilled to welcome you to my portfolio. I am a
          passionate and versatile full-stack developer with a keen interest in
          exploring the latest cutting-edge technologies. My journey in the
          world of web development has been nothing short of exhilarating, and I
          constantly strive to enhance my skills and embrace emerging trends in
          the industry.
        </p>
      </div>
      <div class="skillsHead">What I do!</div>
      <div class="skills">
        <div class="webDev">
          <div class="webDevUp">
            <img src="images/code.svg" alt="code" />
            <span>Web Development</span>
          </div>
          <div class="webDevDown">
            <span>
              As a developer, I find myself most captivated by the power and
              flexibility of NEXT.js. I'm always eager to dive into new projects
              that leverage NEXT.js and discover innovative ways to create fast,
              scalable, and user-friendly applications.
            </span>
          </div>
        </div>
        <div class="appDev">
          <div class="appDevUp">
            <img src="images/app.svg" alt="app" />
            <span>App Development</span>
          </div>
          <div class="appDevDown">
            <span>
              With a focus on user-centric design and cutting-edge technologies,
              I I thrive on building intuitive and efficient apps that make a
              positive impact on people's lives. Let's turn ideas into reality
              the future together.
            </span>
          </div>
        </div>
        <div class="ux">
          <div class="uxUp">
            <img src="images/ux.svg" alt="ux" />
            <span>UI/UX Designing</span>
          </div>
          <div class="uxDown">
            <span>
              Crafting visually appealing and intuitive user interfaces that
              offer offer a delightful user experience is something I'm truly
              about.
            </span>
          </div>
        </div>
        <div class="mentor">
          <div class="mentorUp">
            <img src="images/mentor.svg" alt="mentor" />
            <span>Mentorship</span>
          </div>
          <div class="mentorDown">
            <span
              >I have also found great joy in sharing my knowledge with others.
              Being a technical mentor allows me to give back to the community
              that has supported me throughout my career.
            </span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.containerHome {
  height: 700px;
  margin: 0;
  padding: 0 54px 0 73px;

  .headerHome {
    display: flex;
    flex-direction: row;
    gap: 32px;
    align-items: center;
    justify-content: flex-start;
    .hrHeader {
      width: 252px;
      height: 2px;
      background: linear-gradient(80deg, #ff9c1a 5%, #e80505 100%);
    }
    span {
      color: #0b0909;
      font-family: "Poppins", sans-serif;
      font-size: 42px;
      font-style: normal;
      font-weight: 500;
      line-height: 40px; /* 100% */
      letter-spacing: 1px;
      position: relative;
      left: 2px;
    }
  }
  .infoHome {
    color: #000;
    font-family: "Raleway", sans-serif;
    font-size: 16px;
    font-style: normal;
    font-weight: 500;
    line-height: 30px; /* 187.5% */
    margin-top: 24px;
  }
  .skillsHead {
    color: #000;
    font-family: "Poppins", sans-serif;
    font-size: 32px;
    font-style: normal;
    font-weight: 500;
    line-height: 40px; /* 125% */
    letter-spacing: 0.8px;
    margin-bottom: 30px;
    margin-left: 4px;
  }
  .skills {
    display: flex;
    flex-wrap: wrap;
    gap: 27px;
    .webDev {
      width: 333px;
      height: 169px;
      background: #ffebd1;
      border-radius: 20px;
      .webDevUp {
        display: flex;
        justify-content: flex-start;
        gap: 10px;
        align-items: center;
        margin: 10px 25px 0 25px;
        span {
          color: #000;
          font-size: 24px;
          font-style: normal;
          font-weight: 600;
          line-height: 20px; /* 83.333% */
        }
      }
      .webDevDown {
        margin: 0 25px 10px 25px;
        span {
          color: #000;
          font-size: 14px;
          font-style: normal;
          font-weight: 400;
          line-height: 20px; /* 142.857% */
          letter-spacing: 0.35px;
        }
      }
    }
    .appDev {
      width: 333px;
      height: 169px;
      background: #f2f7fc;
      border-radius: 20px;
      .appDevUp {
        display: flex;
        justify-content: flex-start;
        gap: 10px;
        align-items: center;
        margin: 10px 25px 0 25px;
        span {
          color: #000;
          font-size: 24px;
          font-style: normal;
          font-weight: 600;
          line-height: 20px; /* 83.333% */
        }
      }
      .appDevDown {
        margin: 0 25px 10px 25px;
        span {
          color: #000;
          font-size: 14px;
          font-style: normal;
          font-weight: 400;
          line-height: 20px; /* 142.857% */
          letter-spacing: 0.35px;
        }
      }
    }
    .ux {
      width: 333px;
      height: 169px;
      background: #f2f7fc;
      border-radius: 20px;
      .uxUp {
        display: flex;
        justify-content: flex-start;
        gap: 10px;
        align-items: center;
        margin: 10px 25px 0 25px;
        span {
          color: #000;
          font-size: 24px;
          font-style: normal;
          font-weight: 600;
          line-height: 20px; /* 83.333% */
        }
      }
      .uxDown {
        margin: 0 25px 10px 25px;
        span {
          color: #000;
          font-size: 14px;
          font-style: normal;
          font-weight: 400;
          line-height: 20px; /* 142.857% */
          letter-spacing: 0.5px;
        }
      }
    }
    .mentor {
      width: 333px;
      height: 169px;
      background: #ffebd1;
      border-radius: 20px;
      .mentorUp {
        display: flex;
        justify-content: flex-start;
        gap: 10px;
        align-items: center;
        margin: 10px 25px 0 25px;
        span {
          color: #000;
          font-size: 24px;
          font-style: normal;
          font-weight: 600;
          line-height: 20px; /* 83.333% */
        }
      }
      .mentorDown {
        margin: 0 25px 10px 25px;
        span {
          color: #000;
          font-size: 14px;
          font-style: normal;
          font-weight: 400;
          line-height: 20px; /* 142.857% */
          letter-spacing: 0.35px;
        }
      }
    }
  }
}
</style>
