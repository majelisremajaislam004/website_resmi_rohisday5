<template>
    <main>
        <a class="link" href="https://www.youtube.com/channel/UC6p0zIW56NmMncpIR_Ec-qQ" target="_blank"><h2>SELAYANG PANDANG MA'RIFAT</h2></a>
        <div class="movie_card" id="bright">
          <div class="info_section">
            <div class="movie_header">
              <img class="locandina" src="~/static/assets/img/i.jpg">
              <h1>MA'RIFAT</h1>
              <h4>Majelis Remaja Islam SMKN 4 Tasikmalaya</h4>
              <span class="minutes">002 min</span>
              <p class="type">Documentation</p>
            </div>
            <div class="movie_desc">
              <p class="text">
                Menjelaskan tentang pengenalan atau selayang pandang tentang Ekstrakurikuler MA'RIFAT atau Majelis Remaja Islam SMKN 4 Tasikmalaya.
              </p>
            </div>
            <div class="movie_social">
              <ul>
                <li><i class="material-icons fa fa-share"><a href=""> Share </a></i></li>
                <li><i class="material-icons fa fa-youtube-play"><a href=""> Watch </a></i></li>
                <li><i class="material-icons fa fa-sign-in"><a href=""> Let's Join </a></i></li>
              </ul>
            </div>
          </div>
          <div class="blur_back bright_back"></div>
        </div>

        <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/font-awesome/4.5.0/css/font-awesome.min.css" />
    </main>
</template>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css?family=Montserrat:300,400,700,800');

*{
  box-sizing: border-box;
  margin: 0;
}

html, body{
  margin: 0;
  background: white;
  font-family: 'Montserrat', helvetica, arial, sans-serif;
  font-size: 14px;
  font-weight: 400;
}

.link{
  display: block;
  text-align: center;
  color: #777;
  text-decoration: none;
  padding: 10px;
}

.movie_card{
  position: relative;
  display: block;
  width: 800px;
  height: 350px;
  margin: 80px auto; 
  overflow: hidden;
  border-radius: 10px;
  transition: all 0.4s;
  box-shadow: 0px 0px 120px -25px rgba(0,0,0, 0.5);
  &:hover{
    transform: scale(1.02);
    box-shadow: 0px 0px 80px -25px rgba(0,0,0, 0.5);
    transition: all 0.4s;
  }
  .info_section{
    position: relative;
    width: 100%;
    height: 100%;
	  background-blend-mode: multiply;
    z-index: 2;
    border-radius: 10px;
    .movie_header{
      position: relative;
      padding: 25px;
      height: 40%;
      h1{
        color: black;
        font-weight: 400;
      }
      h4{
        color: #555;
        font-weight: 400;
        font-size: 14px;
      }
      .minutes{
        display: inline-block;
        margin-top: 15px;
        color: #555;
        padding: 5px;
        border-radius: 5px;
        border: 1px solid rgba(0,0,0,0.05);
      }
      .type{
        display: inline-block;
        color: #959595;
        margin-left: 10px;
      }
      .locandina{
        position: relative;
        float: left;
        margin-right: 20px;
        height: 120px;
        box-shadow: 0 0 20px -10px rgba(0,0,0,0.5);
      }
    }
    .movie_desc{
      padding: 25px;
      height: 50%;
      .text{
        color: #545454;
      }
    }
    .movie_social{
      height: 10%;
      padding-left: 15px;
      padding-bottom: 20px;
      ul{
        list-style: none;
        padding: 0;
        li{
          display: inline-block;
          color: rgba(0,0,0,0.3);
          transition: color 0.3s;
          transition-delay: 0.15s;
          margin: 0 10px;
          &:hover{
            transition: color 0.3s;
            color: rgba(0,0,0,0.7);
          }
          i{
            color: #0e62ff;
            font-size: 19px;
            cursor: pointer;
          }
          a{
            text-decoration: none;
          }
        }
      }
    }
  }
  .blur_back{
    position: absolute;
    top: 0;
    z-index: 1;
    height: 100%; right: 0;
    background-size: cover;
    border-radius: 11px;
  }
}

@media screen and (min-width: 768px) {
  .movie_header{
    width: 65%;
  }
  
  .movie_desc{
    width: 50%;
  }
  
  .info_section{
    background: linear-gradient(to right, #e5e6e6 50%, transparent 100%);
  }
  
  .blur_back{
    width: 80%;
    background-position: -100% 10% !important;  
  }
}

@media screen and (max-width: 768px) {
  .movie_card{
    width: 95%;
    margin: 70px auto; 
    min-height: 350px;
    height: auto;
  }
  
  .blur_back{
    width: 100%;
    background-position: 50% 50% !important;  
  }
  
  .movie_header{
    width: 100%;
    margin-top: 85px;
  }
  
  .movie_desc{
    width: 100%;
  }
  
  .info_section{
    background: linear-gradient(to top, #e5e6e6 50%, transparent 100%);
    display: inline-grid;
  }
}


.bright_back{
  background: url("~/static/assets/img/h1 (1).jpg");
}
</style>
