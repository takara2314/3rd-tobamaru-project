<script>
  import MetaTags from "../components/MetaTags.svelte";
  import PrimaryBtn from "../components/buttons/PrimaryBtn.svelte";
  import SecondaryBtn from "../components/buttons/SecondaryBtn.svelte";
  import H2 from "../components/headers/H2.svelte";
  import CommonWave from "../components/waves/CommonWave.svelte";

  const news = [
    {
      name: "第59回鳥羽商船海学祭",
      date: "2024-11-30",
      href: "/news/2024-kaigakusai",
      image: "/news/2024-kaigakusai/image.webp"
    },
    {
      name: "【応募終了】2024鳥羽丸写真コンテストを開催します！",
      date: "2024-10-08",
      href: "/news/2024-photo-contest",
      image: "/news/2024-photo-contest/image.webp"
    },
    {
      name: "【終了】３代目鳥羽丸記念航海乗船者募集",
      date: "2024-05-22",
      href: "/news/tobamaru-final-24",
      image: "/news/tobamaru-final-24/image.webp"
    },
    {
      name: "練習船「鳥羽丸」体験航海参加者募集",
      date: "2024-05-09",
      href: "/news/tobamaru-taiaken-24",
      image: "/news/tobamaru-taiaken-24/image.webp"
    },
    {
      name: "学校だよりの表紙にフォトコンテスト受賞作品が掲載されました",
      date: "2023-12-30",
      href: "/news/school-newsletter-95",
      image: "/news/school-newsletter-95/newsletter-cover.webp"
    },
    {
      name: "【結果発表】2023鳥羽丸写真コンテストの結果発表",
      date: "2023-12-30",
      href: "/news/2023-photo-contest-results",
      image: "/news/2023-photo-contest-results/1st-award.webp"
    },
    {
      name: "新しい鳥羽丸の情報が日経新聞で紹介されました",
      date: "2023-11-10",
      href: "/news/new-tobamaru-nikkei",
      image: "/news/new-tobamaru-nikkei/image.webp"
    },
    {
      name: "ホームページをリニューアルしました",
      date: "2023-10-20",
      href: "/news/hp-renewal",
      image: "/photos/tobamaru.webp"
    },
    {
      name: "【応募終了】2023鳥羽丸写真コンテストを開催します！",
      date: "2023-10-08",
      href: "/news/2023-photo-contest",
      image: "/photos/commemorative-photo.webp"
    },
    {
      name: "第一回 鳥羽丸見学を実施しました",
      date: "2023-04-21",
      href: "/news/1st-tobamaru-visit",
      image: "/photos/looking.webp"
    }
  ];

  const events = [
    {
      name: "第59回鳥羽商船海学祭",
      date: ["2024-11-30 ～ 12-01"],
      target: ["鳥羽商船学生", "一般"],
      comment: "",
      href: "/news/2024-kaigakusai"
    },
    {
      name: "【応募終了】2024鳥羽丸写真コンテスト",
      date: ["2024-10-08 ～ 10-31"],
      target: ["鳥羽商船学生", "一般"],
      comment: "",
      href: "/news/2024-photo-contest"
    },
    {
      name: "【終了】３代目鳥羽丸記念航海乗船者募集",
      date: ["2024-05-21 ～ 05-30"],
      target: ["鳥羽商船学生"],
      comment: "",
      href: "/news/tobamaru-final-24"
    },
    {
      name: "第58回海学祭　模擬店",
      date: ["2023-12-02 ～ 12-03"],
      target: ["鳥羽商船学生", "一般"],
      comment: "写真コンテストの表彰も実施",
      href: "https://gakuseikai.toba-cmt.ac.jp/kaigakusai/"
    },
    {
      name: "【応募終了】2023鳥羽丸写真コンテスト",
      date: ["2023-10-08 ～ 11-08"],
      target: ["鳥羽商船学生"],
      comment: "",
      href: "/news/2023-photo-contest"
    }
  ];
</script>

<svelte:head>
  <script src="https://snapwidget.com/js/snapwidget.js" />
</svelte:head>

<MetaTags
  title="Tobamaru Project Team"
  description="Tobamaru Project Teamは、代船入替えに向けて記念行事、在校生や卒業生の鳥羽商船に対する愛着や地域の人々の親しみをより深めるための企画を検討する学生団体です。"
  href="/"
/>

<header>
  <!-- svelte-ignore a11y-media-has-caption -->
  <video autoplay muted loop preload="none">
    <source src="/web-promotion.webm" type="video/webm" />
    <source src="/web-promotion.mp4" type="video/mp4" />
  </video>

  <div class="header-wave">
    <CommonWave />
  </div>

  <section class="scroll-down-area">
    <div class="scroll-down">
      <span class="arrow-down" />
      <span class="scroll-title">
        Scroll down
      </span>
    </div>
  </section>
</header>

<main>
  <section id="whats-tobamaru" class="column-2">
    <figure class="left-image">
      <img
        src="/photos/tobamaru.webp"
        alt="鳥羽丸"
      />
      <figcaption>
        撮影者:　福野 泰介様
      </figcaption>
    </figure>

    <article>
      <H2>
        鳥羽丸とは？
      </H2>
      <div>
        <p>
          鳥羽丸（とばまる）とは、
          鳥羽商船高等専門学校が保有する練習船です。
        </p>
        <p>
          現在は1994年に建造された3代目が運用されており、
          主に商船学科の学生の航海実習に使用されています。
        </p>
        <p>
          これまで、多くの方の記憶に刻まれていた
          3代目鳥羽丸は2024年06月14日に大勢に見送られながら引退セレモニーを行いました
        </p>
      </div>

      <!-- <PrimaryBtn
        label="詳しいプロフィールを見る！"
        href="/3rd-tobamaru"
      /> -->
    </article>
  </section>

  <section id="news">
    <article>
      <H2>ニュース</H2>
      <div>
        鳥羽丸とTobamaru Project Teamについての最新情報を掲載します
      </div>
    </article>
    <div class="news">
      <ul>
        {#each news as article}
          <li>
            <a href={article.href}>
              <img
                src={article.image}
                alt={article.name}
              />
              <div>
                <div>
                  <span class="published-at">
                    {article.date}
                  </span>
                </div>
                <h3>
                  {article.name}
                </h3>
              </div>
            </a>
          </li>
        {/each}
      </ul>
    </div>
  </section>

  <div class="blue-bg-area">
    <section id="events" class="column-2">
      <article>
        <H2 whiteWave>
          イベント
        </H2>
        <div>
          不定期に鳥羽丸に関するイベントを開催しています
        </div>

        <ul class="events">
          {#each events as event}
            <li>
              <a href={event.href}>
                <button aria-label={event.name}>
                  <h3>
                    {event.name}
                  </h3>
                  <div class="date">
                    {event.date[0]}
                    {#if event.date.length > 1}
                      <span>・</span>
                      {event.date[1]}
                    {/if}
                  </div>
                  <ul class="badge">
                    <li class="target">
                      対象: {event.target.join(", ")}
                    </li>
                    {#if event.comment !== ""}
                      <li class="comment">
                        {event.comment}
                      </li>
                    {/if}
                  </ul>
                </button>
              </a>
            </li>
          {/each}
        </ul>
      </article>

      <figure class="right-image">
        <img
          src="/photos/looking.webp"
          alt="望遠鏡を見る女の子"
        />
      </figure>
    </section>

    <section id="instagram">
      <article>
        <H2 whiteWave>
          Instagram
        </H2>
        <div>
          定期的に鳥羽丸や鳥羽商船にまつわる情報を投稿します
        </div>
      </article>
      <iframe
        title="Instagramの投稿"
        src="https://snapwidget.com/embed/1017460"
        class="snapwidget-widget instagram-feed"
      />
    </section>
  </div>

  <section id="whats-tobamaru-project-team" class="column-2">
    <figure class="left-image">
      <img
        src="/photos/commemorative-photo.webp"
        alt="集合写真"
      />
    </figure>

    <article>
      <H2>
        Tobamaru Project Teamとは？
      </H2>

      <div>
        <p>
          Tobamaru Project Teamは、
        </p>
        <p>
          代船入替えに向けて記念行事、
        </p>
        <p>
          在校生や卒業生の鳥羽商船に対する愛着や
        </p>
        <p>
          地域の人々の親しみをより深めるための
        </p>
        <p>
          企画を検討する学生団体です。
        </p>
        <p>
          （学校から結成承認済み）
        </p>
      </div>

      <div class="button-column">
        <p>
          <SecondaryBtn
            label="活動規約"
            href="/terms.pdf"
          />
        </p>
        <p>
          <PrimaryBtn
            label="詳しく!(入会はこちらから)"
            href="/joinus"
          />
        </p>
      </div>
    </article>
  </section>
</main>

<style>
  header {
    width: 100dvw;
    height: 90dvh;
    background-color: black;
    position: relative;
    overflow: hidden;
  }

  header video {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: top 0 right -40vw;
  }

  .header-wave {
    width: 100%;
    color: var(--bg-color);
    display: flex;
    flex-direction: column;
    position: absolute;
    left: 0;
    bottom: 0;
  }

  .header-wave::after {
    content: "";
    width: 100%;
    height: 0.5rem;
    background-color: var(--bg-color);
    position: absolute;
    bottom: -0.2rem;
  }

  .scroll-down-area {
    width: 8rem;
    height: 10rem;
    position: absolute;
    bottom: -15rem;
    right: 0;
  }

  .scroll-down {
    display: block;
    position: relative;
    padding-top: 5.5rem;
    text-align: center;
  }

  .arrow-down {
    display: block;
    margin: 0 auto;
    width: 0.5rem;
    height: 1rem;
  }

  .arrow-down:after {
    content: '';
    display: block;
    margin: 0;
    padding: 0;
    width: 0.5rem;
    height: 0.5rem;
    border-top: 0.15rem solid var(--bg-color);
    border-right: 0.15rem solid var(--bg-color);
    transform: rotate(135deg);
  }

  .scroll-title {
    display: block;
    text-transform: uppercase;
    color: var(--bg-color);
    font-size: 0.75rem;
    font-weight: bold;
    letter-spacing: 0.1rem;
    rotate: 90deg;
    transform: translate(-4.25rem, -1.5rem);
  }

  .scroll-down::before {
    animation: elasticus 1.5s cubic-bezier(1, 0, 0, 1) infinite;
    position: absolute;
    top: 0;
    left: 50%;
    margin-left: -0.1rem;
    width: 0.15rem;
    height: 5.5rem;
    background: var(--bg-color);
    content: ' ';
  }

  @keyframes elasticus {
    0% {
      transform-origin: 0% 0%;
      transform: scale(1, 0);
    }

    50% {
      transform-origin: 0% 0%;
      transform: scale(1, 1);
    }

    50.1% {
      transform-origin: 0% 100%;
      transform: scale(1, 1);
    }

    100% {
      transform-origin: 0% 100%;
      transform: scale(1, 0);
    }
  }

  main {
    min-height: auto;
    margin: auto;
  }

  .blue-bg-area {
    background-color: var(--section-bg-color);
    display: flex;
    flex-direction: column;
    align-items: center;
    position: relative;
  }

  .blue-bg-area::before {
    content: "";
    width: 100%;
    height: 10rem;
    background-color: var(--bg-color);
    position: absolute;
    top: 0;
    clip-path: polygon(0 0, 0 50%, 50% 0, 100% 50%, 100% 0);
  }

  .blue-bg-area::after {
    content: "";
    width: 100%;
    height: 10rem;
    background-color: var(--bg-color);
    position: absolute;
    bottom: 0;
    clip-path: polygon(0 100%, 0 50%, 50% 100%, 100% 50%, 100% 100%);
  }

  .button-column {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .button-column p {
    margin-bottom: 2rem;
  }

  .news {
    width: 90vw;
    height: 22rem;
    margin-top: 2rem;
    overflow-x: auto;
  }

  .news ul {
    height: calc(100% - 0.5rem);
    display: grid;
    grid-auto-flow: column;
    gap: 2.5rem;
  }

  .news ul > li {
    width: 25rem;
    height: 100%;
  }

  .news a {
    width: 100%;
    height: 100%;
    border-radius: 1rem;
    text-align: left;
    background-color: var(--primary-btn-bg-color);
    box-shadow: 0 0.25rem 0.1rem var(--primary-btn-shadow-color);
    overflow: hidden;
    display: block;
  }

  .news a > img {
    width: 100%;
    height: 15rem;
    object-fit: cover;
  }

  .news a > div {
    width: 100%;
    height: calc(100% - 15rem);
    padding: 0.25rem 1rem;
  }

  .news .published-at {
    color: var(--primary-color);
    font-size: 1rem;
    padding: 0.1rem 2rem;
    background-color: var(--bg-color);
    border-radius: 0.5rem;
  }

  .news h3 {
    color: var(--primary-color);
    text-align: center;
    margin-top: 0.25rem;
  }

  .events {
    width: 100%;
    padding: 1rem;
    display: flex;
    flex-direction: column;
  }

  .events > li {
    width: 100%;
    margin-bottom: 1rem;
  }

  .events > li > a > button {
    width: 100%;
    text-align: left;
    background-color: var(--bg-color);
    box-shadow: 0 0.25rem 0.1rem var(--primary-btn-shadow-color);
    padding: 1rem;
    border-radius: 1rem;
  }

  .events h3 {
    color: var(--primary-color);
    margin-bottom: 0.5rem;
  }

  .events .date {
    margin-bottom: 0.5rem;
    font-size: 1rem;
  }

  .events .badge {
    font-size: 1rem;
    display: flex;
    flex-direction: row;
  }

  .events .badge > * {
    margin-right: 1rem;
    padding-left: 1rem;
    padding-right: 1rem;
  }

  .events .target {
    background-color: var(--secondary-btn-bg-color);
    border-radius: 1rem;
  }

  .events .comment {
    color: rgb(239, 68, 68);
    background-color: var(--secondary-btn-bg-color);
    border-radius: 1rem;
  }

  .instagram-feed {
    width: 100vw;
    height: 100vw;
    background-color: var(--bg-color);
    margin-top: 2rem;
    padding: 1rem;
    border: none;
    border-radius: 1rem;
  }

  @media (min-width: 1024px) {
    header {
      width: 100%;
      height: 98dvh;
      background-color: black;
      position: relative;
    }

    header video {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: top 0 right 0;
    }

    .scroll-down-area {
      width: 8rem;
      height: 10rem;
      position: absolute;
      bottom: -12rem;
      right: 1rem;
    }

    .blue-bg-area::before {
      content: "";
      width: 100%;
      height: 10rem;
      background-color: var(--bg-color);
      position: absolute;
      top: 0;
      clip-path: polygon(0 0, 0 100%, 50% 0, 100% 100%, 100% 0);
    }

    .blue-bg-area::after {
      content: "";
      width: 100%;
      height: 10rem;
      background-color: var(--bg-color);
      position: absolute;
      bottom: 0;
      clip-path: polygon(0 100%, 0 0, 50% 100%, 100% 0, 100% 100%);
    }

    .news {
      width: 90vw;
      height: 23.5rem;
      margin-top: 2rem;
      overflow-x: auto;
    }

    .events {
      width: 100%;
      display: flex;
      flex-direction: column;
    }

    .instagram-feed {
      width: 80vw;
      height: 80vw;
      background-color: var(--bg-color);
      margin-top: 2rem;
      padding: 1rem;
      border: none;
      border-radius: 1rem;
    }
  }
</style>
