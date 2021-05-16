<template>
  <main>
    <section class="brand">
      <div>
        <img :src="require('~/static/cs.png')" alt="IEEE Ankara Computer Society">
        <span class="bubble">Komitemize Hoş Geldiniz !</span>
        <NuxtLink class="forward" to="/iletisim">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="icon icon-tabler icon-tabler-mail"
            width="24"
            height="24"
            viewBox="0 0 24 24"
            stroke-width="2"
            stroke="currentColor"
            fill="none"
            stroke-linecap="round"
            stroke-linejoin="round"
          >
            <path stroke="none" d="M0 0h24v24H0z" fill="none" />
            <rect x="3" y="5" width="18" height="14" rx="2" />
            <polyline points="3 7 12 13 21 7" />
          </svg>
          <span>Bize Katıl</span>
        </NuxtLink>
      </div>
    </section>
    <section class="section">
      <article id="">
        <div class="content">
          <div class="text">
            <h2>Biz Kimiz ? </h2>
            <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Delectus incidunt veritatis repudiandae reprehenderit fugiat officiis deleniti harum tenetur id illum repellat, illo laboriosam aperiam cupiditate distinctio temporibus explicabo enim accusamus itaque aliquam blanditiis animi quasi natus. Impedit fugit excepturi sit quaerat, maxime, nisi natus incidunt sed, cumque corrupti rem consequatur aut accusamus harum. Vel optio et autem, aliquid molestiae quis accusantium consequuntur totam ducimus. Repudiandae temporibus numquam perspiciatis voluptates! Quas quam distinctio cum. Ex aliquid sint, labore iste aspernatur ea.</p>
          </div>
        </div>
      </article>
    </section>
    <section class="section">
      <article id="">
        <div class="content">
          <div class="text">
            <h2>Yönetim</h2>
            <div class="yonetim">
              <div class="card">
                <figure>
                  <img src="https://dummyimage.com/500.png" alt="">
                  <figcaption>
                    <h4>İsim</h4>
                    <small>Yetki</small>
                    <div class="sosyal">
                      <span>ico</span>
                      <span>ico</span>
                      <span>ico</span>
                    </div>
                  </figcaption>
                </figure>
              </div>
              <div class="card" />
              <div class="card" />
            </div>
          </div>
        </div>
      </article>
    </section>
    <section class="section">
      <article id="">
        <div class="content">
          <div class="text">
            <h2>Ekiplerimiz</h2>
            <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Delectus incidunt veritatis repudiandae reprehenderit fugiat officiis deleniti harum tenetur id illum repellat, illo laboriosam aperiam cupiditate distinctio temporibus explicabo enim accusamus itaque aliquam blanditiis animi quasi natus. Impedit fugit excepturi sit quaerat, maxime, nisi natus incidunt sed, cumque corrupti rem consequatur aut accusamus harum. Vel optio et autem, aliquid molestiae quis accusantium consequuntur totam ducimus. Repudiandae temporibus numquam perspiciatis voluptates! Quas quam distinctio cum. Ex aliquid sint, labore iste aspernatur ea.</p>
          </div>
        </div>
      </article>
    </section>
  </main>
</template>

<script>
export default {

}
</script>

<style scoped lang="scss">
$ieee-orange: #FFA300;
$ieee-blue: #00629b;
$ieee-cyan: #00b5e2;
$ieee-black: #000000;
$ieee-white: #ffffff;
$ieee-grey: #75787b;
main{
  section{
    display: grid;
    place-content: center;
    height: 100vh;
    width: 100%;
    &.brand{
        svg{
          height: 1.5em;
          width:1.5em;
      }
      div{
        display: grid;
        row-gap: 0;
      }
      .forward{
        &:hover{
          svg{
            color:$ieee-blue;
            animation-name: bounce;
            animation-iteration-count: infinite;
            animation-duration: 1s;
            animation-timing-function: cubic-bezier(0.455, 0.03, 0.515, 0.955);
          }
          transition: all 0.56s cubic-bezier(0.075, 0.82, 0.165, 1) 0s;
        }
        margin-top: 4rem;
        background: white;
        color: black;
        svg{
          margin-left: .3em ;
          height: .7em;
          width: .7em;
        }
        border: $ieee-black solid .1em;
        padding: .2em;
        text-align: center;
        border-radius: 4rem;
      }
      font-size: 2.5rem;
      place-content: center;
      display: grid;
      color: $ieee-black ;
      text-transform: capitalize;
      text-align: left;
      //background-color: #75787b;
      //background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='20' height='12' viewBox='0 0 20 12'%3E%3Cg fill-rule='evenodd'%3E%3Cg id='charlie-brown' fill='%23ffffff' fill-opacity='1'%3E%3Cpath d='M9.8 12L0 2.2V.8l10 10 10-10v1.4L10.2 12h-.4zm-4 0L0 6.2V4.8L7.2 12H5.8zm8.4 0L20 6.2V4.8L12.8 12h1.4zM9.8 0l.2.2.2-.2h-.4zm-4 0L10 4.2 14.2 0h-1.4L10 2.8 7.2 0H5.8z'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E");
      background-color: #ffffff;
      background-image: url("data:image/svg+xml,%3Csvg width='20' height='20' viewBox='0 0 20 20' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='%23ffa300' fill-opacity='1' fill-rule='evenodd'%3E%3Ccircle cx='3' cy='3' r='3'/%3E%3Ccircle cx='13' cy='13' r='3'/%3E%3C/g%3E%3C/svg%3E");
      img,.bubble{border:3px solid $ieee-black}
          img{
            font-size: 2em ;
            background: #fff;
            padding: 1rem;
            border-radius: 4em 4em 4em 0;
            width: max-content;
          }
          .mail{
            position: fixed;
            bottom: 1rem;
            right: 3rem;
            img{
              border: $ieee-black;
              background: #75787b;
            }
          }
          .bubble{
            background: #fff;
            padding: 1rem;
            border-radius: 0 4em 4em 4em ;
            width: max-content;
            font-size:1em;
          }
    }
    &.section{
        place-content: center;
        height: 75vh;
      .content{
        display: grid;
        grid-template-columns: 1fr 1fr;
        margin: auto 4rem;
      }
    }

  }
}
    @keyframes bounce {
        0%   { transform: translateY(0); }
        50%  { transform: translateY(-40%); }
        100% { transform: translateY(0); }
    }
</style>
