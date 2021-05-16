<template>
  <nav>
    <div class="logo">
      <NuxtLink to="/">
        <img :src="require('~/static/logo.png')" alt="IEEE ANKARA UNIVERSITY" srcset="">
      </NuxtLink>
    </div>
    <div class="duyuru">
      <span><NuxtLink to="/theduyuru">Küçük bir duyuru arasına girelim</NuxtLink></span>
    </div>
    <div class="nav">
      <ul>
        <li>
          <NuxtLink style="color:inherit" class="nav__link" to="/">
            Ana Sayfa
          </NuxtLink>
        </li>
        <li>
          <NuxtLink class="nav__link" to="/hakkimizda">
            Hakkımızda
          </NuxtLink>
        </li>
        <li>
          <div class="down">
            <NuxtLink class="nav__link drop" to="/komiteler">
              Komitelerimiz
            </NuxtLink>
            <div class="down__links">
              <NuxtLink class="nav__link" to="/komiteler/aess">
                Aerospace and Electronic Systems Society.
              </NuxtLink>
              <NuxtLink class="nav__link" to="/komiteler/cs">
                Computer Society
              </NuxtLink>
              <NuxtLink class="nav__link" to="/komiteler/embs">
                Engineering in Medicine and Biology Society
              </NuxtLink>
              <NuxtLink class="nav__link" to="/komiteler/pes">
                Power and Energy Society
              </NuxtLink>
              <NuxtLink class="nav__link" to="/komiteler/ras">
                Robotics and Automation Society
              </NuxtLink>
              <NuxtLink class="nav__link" to="/komiteler/wie">
                Women in Engineering
              </NuxtLink>
            </div>
          </div>
        </li>
        <li>
          <NuxtLink class="nav__link" to="/etkinlikler">
            Etkinlikler
          </NuxtLink>
        </li>
        <li>
          <NuxtLink class="nav__link" to="/iletisim">
            İletişim
          </NuxtLink>
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
$ieee-orange: #FFA300;
$ieee-blue: #00629b;
$ieee-cyan: #00b5e2;
$ieee-black: #000000;
$ieee-white: #ffffff;
$ieee-grey: #75787b;
@import url('https://fonts.googleapis.com/css2?family=Montserrat&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Lexend+Deca&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Source+Sans+Pro&display=swap');
nav{
  border-bottom: 3px solid $ieee-black;
  background: #fff;
  color:$ieee-black;
  width: 100%;
  display: flex ;
  justify-content: space-evenly ;
  height: 10vh;
  align-items: center;
  text-align: center;
  position: fixed;
  top: 0;
  .logo{
    margin-left: 2rem;
    margin-right: 2rem;
    a {
      text-decoration: none;
      text-align: center;
      color:inherit;
    }
    img{
      height: 6vh;
    }
  }
  .nav{
    font-size: 1.1rem;
    font-weight: bold;
    color:inherit;
    display: flex;
    margin-left: 2rem;
    margin-right: 2rem;
      ul {
        display: flex;
        li{
          &:first-child{margin-left: 0;}
          margin-left: 1rem;
          list-style: none;
          a {
              color:inherit;
              transition: all 0.1s ease 0.04s;
              text-decoration: none;
              &:hover{
                color: $ieee-blue
              }
              &:active{
                color:$ieee-blue;
              }
            }
          .nuxt-link-active{
            color:$ieee-blue
          }
          .nuxt-exact-link-active{
            color:$ieee-blue
          }
          .down{
            display: inline-block;
            position: relative;
            .drop::after{
              content: "▼";
            }
            .down__links{
              background: #fff;
              font-weight: initial ;
              display: none;
              position: absolute;
              border: $ieee-blue 2px solid;

              a:hover{
                background: $ieee-blue;
                color:$ieee-white
              }
              a{
                padding: 0.4rem;
                display: block;
                border-bottom: #00629b 1px solid;
              }
            }
            &:hover .down__links{
              display: block;
            }
          }
        }
      }
}
  .duyuru{
    margin-left: 2rem;
    margin-right: 2rem;
    width: 25%;
    color:blue;
    &::before{
      content: "#";
    }
    span{
      a{
        &:active{
          color: red;
        }
        color:inherit;
      }
    }
  }
}

</style>
