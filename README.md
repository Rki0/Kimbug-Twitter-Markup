# ๐ Twitter Markup (HTML sectioning tag)

<img src="https://user-images.githubusercontent.com/86224851/155629398-5b5bd475-310a-4d67-a36f-469c6ef2f29c.jpeg">

ํธ์ํฐ ํํ์ด์ง์ HTML ๋ฌธ์๋ฅผ ์์ฑํ  ๋ ์ด๋ค ์์ผ๋ก ๊ตฌํ์ ๋๋๊ณ  ๊ฐ๊ฐ์ ์์๋ค์ ๊ตฌํํ๋์ง์ ๋ํด์ ์ดํด๋ณด๋ฉด์, HTML sectioning tag์ ๋ํด ๊ณต๋ถํ์.  
HTML์ ๊ตฌํ์ ๋ํ ๊ณต๋ถ์ด๋ฏ๋ก CSS์ JS๋ ์ธ๊ธํ์ง์๋๋ค.

๊ธฐ๋ณธ์ ์ผ๋ก ์๊ณ  ๊ฐ์ผํ  ๊ฒ์ด ์๋ค.  
sectioning tag์๋ section, article, nav, aside๊ฐ ์๋ค.  
์ด๋ค์ ์ฌ์ฉ ํ ๋ฐ๋์ heading ํ๊ทธ(h ํ๊ทธ)๋ฅผ ์ฌ์ฉํด์ ์ ๋ชฉ์ ํ์ํด์ค์ผํ๋ค.  
๊ทธ๊ฒ ์ฌ์ฉ์์๊ฒ ๋ณด์ด๋ ๋ถ๋ถ์ด๋  ์๋๋  ๊ผญ!

## ๐ header

<img width="483" alt="แแณแแณแแตแซแแฃแบ 2022-02-25 แแฉแแฅแซ 9 30 48" src="https://user-images.githubusercontent.com/86224851/155630602-960cb2da-8192-4346-b9e4-1b78222d3fe2.png">

๋ณดํต ์ผ๋ฐ์ ์ธ ์ฌ์ดํธ์ ๊ฒฝ์ฐ ํ์ฌ ๋ก๊ณ ์ ๋ฉ๋ด๋ฐ๊ฐ ์์ชฝ์ ์์ด header๋ก ์๊ฐํ๊ธฐ ํธํ๋ฐ, ํธ์ํฐ์ ๊ฒฝ์ฐ ์ธ๋ก๋ก ๋ถํ ๋์ด ์์ด ์ฝ๊ฐ ์ ์ ํ๋ค.  
ํํ๋ง ๋ฌ๋ผ์ก์ ๋ฟ์ด๋ฏ๋ก ๋ถ์์ ํ์ ๋ถ๋ถ์ **header**๋ก ๋ฌถ์ด์ฃผ๊ฒ ๋ค.

๋ก๊ณ  ๋ถ๋ถ๊ณผ ๋ฉ๋ด๋ฐ ๋ถ๋ถ์ ํด๋น ํ์ด์ง๋ก ์ด๋ํ๊ฑฐ๋ ์ถ๊ฐ ๋ฉ๋ด๋ฅผ ๋ณด์ฌ์ฃผ๋ ๋ฑ ๊ธฐ๋ฅ์ ๋น์ทํ๋ค.  
ํ์ง๋ง ๋ก๊ณ ์ ๊ฒฝ์ฐ ํ์ด์ง๋ฅผ ๋ํํ๋ ๋๋์ด ์์ผ๋ฏ๋ก ๋ฐ๋ก ์์ฑํ๋ ๊ฒ์ผ๋ก ํ์.

```html
<header>
  <!--ํ์ฌ ๋ก๊ณ -->
  <h1>
    <a href="#">
      <img src="#" alt="Twitter" />
    </a>
  </h1>
</header>
```

h1 ํ๊ทธ๋ฅผ ์ฌ์ฉํด์ ๋ํ์ฑ์ ๊ฐ์กฐํด์คฌ๊ณ , ๋ก๊ณ  ์ด๋ฏธ์ง๋ฅผ ํด๋ฆญํ๋ฉด ํํ์ด์ง๋ก ์ด๋ํ๋ฏ๋ก a ํ๊ทธ๋ก ๊ฐ์ธ์ฃผ์๋ค.

## ๐ nav

๋ค์์ผ๋ก๋ ๋ฉ๋ด๋ฐ๋ฅผ ๋ง๋ค ๊ฒ์ด๋ค.  
๋ฌธ์ ํ์ด์ง ๊ฐ ์ด๋ํ๋ ๊ฒ์ด ์๋ ๊ฒฝ์ฐ **nav** ํ๊ทธ๋ฅผ ์ฌ์ฉํ๋ค.

```html
<nav>
  <h1>Menu</h1>
  <ul>
    <li>
      <a href="#">
        <span>Current page</span>
        Home</a
      >
    </li>
    <li><a href="#">Explore</a></li>
    <li>
      <a href="#">
        <strong aria-label="5 unread notifications">5</strong>
        Notifications</a
      >
    </li>
    <li><a href="#">Messages</a></li>
    <li><a href="#">Bookmarks</a></li>
    <li><a href="#">Lists</a></li>
    <li><a href="#">Profile</a></li>
    <li>
      <button type="button">
        More
        <!--Dropdown Menu-->
      </button>
    </li>
  </ul>
  <button type="button">Tweet</button>
</nav>
```

**nav**๋ sectioning tag์ด๋ฏ๋ก ์ฌ์ฉ ํ heading ํ๊ทธ๋ฅผ ์ฌ์ฉํ์ฌ ์ ๋ชฉ์ ๋ฌ์์คฌ๋ค.  
๋ฉ๋ด๋ฐ์ ๋ค์ด๊ฐ ์์๋ค์ ์์์์ด ๋์ด๋ ๋ฆฌ์คํธ์ด๋ฏ๋ก **ul**์ ์ฌ์ฉํ์ฌ, ๊ฐ๊ฐ์ **li**๋ก ๋ง๋ค์ด์คฌ๋ค.  
ul์ ์ง๊ณ ์์์ผ๋ก li๋ง์ ๋ฐ์ผ๋ฏ๋ก a ํ๊ทธ๋ฅผ ์ฌ์ฉํ๊ณ  ์ถ๋ค๋ฉด li ์์ ์์ฑํด์ผํ๋ค.  
Home ๋ฉ๋ด์๋ span์ ์ฌ์ฉํด์ ์ด ๋ถ๋ถ์ด ์ด๋ค ์๋ฏธ๋ฅผ ๊ฐ์ง๊ณ  ์๋์ง ์ค๋ช์ ์์ฑํ๋ค. span์ ์ผ๋ง๋ ์ง CSS๋ก ์ง์ธ ์ ์์ผ๋...  
Notifications๋ผ๋ ๋ฉ๋ด์๋ 5๊ฐ์ ์๋ก์ด ์๋์ด ์๋ค๋ ํ์๊ฐ ์๋๋ฐ, ์ด๋ ์ฌ์ฉ์์๊ฒ ๊ฐ์กฐํด์ผํ  ๋ถ๋ถ์ด๋ฏ๋ก **strong**์ ์ฌ์ฉํด์ ํ์ํด์คฌ๋ค.  
More ๋ฉ๋ด๋ ํด๋ฆญ ์ Dropdown menu๊ฐ ์์ฑ๋๋ค. ๋ฐ๋ผ์ a๊ฐ ์๋ button ํ๊ทธ๋ฅผ ์ฌ์ฉํ๋ค.

## ๐ main

main ํ๊ทธ๋ html ๋ฌธ์์์ ๋จ ํ๋ฒ๋ง ์ฌ์ฉ ๊ฐ๋ฅํ ํ๊ทธ๋ก, ์น ํ์ด์ง์ ์ฃผ๋ ๋ด์ฉ์ด ๋ณด์ฌ์ง ๋ถ๋ถ์ด๋ค.

<img width="621" alt="แแณแแณแแตแซแแฃแบ 2022-02-25 แแฉแแฅแซ 10 01 02" src="https://user-images.githubusercontent.com/86224851/155633566-876b6baf-4930-4715-ba07-fdf216409c2c.png">

๋ถ์ ์์ผ๋ก ํ์ํด๋์ ๋ถ๋ถ์ ์๋จ์ ๋์ ํธ์์ ์ ๋ ๊ณณ๊ณผ ํ๋จ์ ๊ฒ์๋ฌผ๋ค์ด ๋ณด์ธ๋ค.  
์ฌ์ฉ์๊ฐ ์ฃผ๋ก ์ฌ์ฉํ๋ ๋ถ๋ถ์ด๋ฏ๋ก ์ด๋ฅผ **main** ํ๊ทธ๋ก ๋ฌถ์ด์ฃผ๋๋ก ํ๊ฒ ๋ค.  
์ฐ์ , Home ํ์๊ฐ ์๋ ๋ถ๋ถ์ ์ดํด๋ณด์.  
Home์ด๋ผ๋ ์ ๋ชฉ๊ณผ ์ด๋ค ๋ฒํผ์ด ์๋ค.  
์ด ๋ฒํผ์ ํด๋ฆญ ์ Dropdown menu๊ฐ ๋์จ๋ค.

```html
<main>
  <header>
    <h1>Home</h1>
    <button type="button" aria-label="Timeline options">
      <!--icon-->
    </button>
    <!--Dropdown menu-->
    <div>
      <h2>Home shows you top Tweets first</h2>
      <button type="button">
        <strong> See latest Tweets instead </strong>
        <span> ์ฌ๋ผ์ค๋ ์์๋๋ก ํธ์์ด ํ์๋ฉ๋๋ค. </span>
      </button>
      <a href="#">
        <!--icon-->
        ์ฝํ์ธ  ํ๊ฒฝ์ค์  ๋ณด๊ธฐ
      </a>
    </div>
  </header>
</main>
```

main ์ค์์๋ ์๋ถ๋ถ์ ์กด์ฌํ๋ฏ๋ก header๋ฅผ ์ฌ์ฉํด์ ์์ฑํ๋ค.
button์ ํด๋ฆญ ์ ๋ณด์ฌ์ค Dropdown menu๋ฅผ div๋ฅผ ํ์ฉํด ๋ณ๋๋ก ๋ฌถ์ด๋์ ๊ฒ์ ๋ณผ ์ ์๋ค.

## ๐ section

๋ค์์ผ๋ก๋ ๋์ ํธ์์ ์์ฑํ๋ ๊ณณ์ ์ดํด๋ณด์.  
์ด ๋ถ๋ถ์ ํ์คํธ๋ฅผ ์์ฑํ๋ ๊ณณ์ผ๋ก ๊ทธ ๋ผ๋ฆฌ์ ์ธ ๊ตฌ๋ถ์ด ๋ชํํ๊ฒ ๋ค๋ฅธ ๊ณณ๊ณผ ๊ตฌ๋ณ๋  ์ ์์ผ๋ฏ๋ก **section**์ ํตํด ๊ตฌํ์ ๋ฌถ์ด์ฃผ์๋ค.

```html
<section>
  <h1>Write a Tweet</h1>
  <form action="#" method="post">
    <img src="#" alt="@user" />

    <textarea
      name=""
      id=""
      cols="30"
      rows="10"
      maxlength="280"
      placeholder="What's happening?"
    ></textarea>

    <button type="button" aria-label="Upload files">
      <!--icon-->
    </button>
    <input type="file" multiple accept="image/*, video/*" />

    <button type="button" aria-label="Choose GIFs...">
      <!--icon-->
    </button>

    <button type="button" aria-label="Create a poll">
      <!--icon-->
    </button>

    <button type="button" aria-label="Choose emoji">
      <!--icon-->
    </button>

    <strong aria-label="0 out of 280 characters"> </strong>

    <button type="button" aria-label="add another tweet">
      <!--icon-->
    </button>

    <button type="submit" aria-label="Submit Tweet">Tweet</button>
  </form>
</section>
```

**section** ํ๊ทธ๋ sectioning tag์ด๋ฏ๋ก h ํ๊ทธ๋ฅผ ์ฌ์ฉํด์ ์ ๋ชฉ์ ์ ์ด์คฌ๋ค.  
ํธ์์ ์์ฑํ๋ ๋ถ๋ถ์ ๋ณด๋ฉด ์ด๋ฏธ์ง์ ํ์คํธ ์๋ ฅ๋ถ, ๊ฐ์ข ๊ธฐ๋ฅ์ ๋ฒํผ์ด ์๋ค.  
์ด๋ค์ ๊ฐ๊ฐ์ด ์ฐ๊ฒฐ๋์ด ์๋ ๋์์ ํ๋ฏ๋ก ํ๋์ form ํ๊ทธ ์์ ๋ฃ์ด์ฃผ๋ ๊ฒ์ด ์ข์ ๊ฒ ๊ฐ๋ค.  
ํ๋จ์ ๋ค์ํ ๊ธฐ๋ฅ์ ํ๋ ๋ฒํผ๋ค์ด ๋ณด์ธ๋ค.  
์ค๋ช์ "button"์ด๋ผ๊ณ  ํ์ง๋ง ์ค์  ํ์ผ์ ์ฝ์ํ๋ ๋ฑ์ ๊ธฐ๋ฅ์ "input"์ ํตํด ๊ตฌํํ๋ค.  
๋ฌธ์ ๋ input ํ๊ทธ๋ ๊พธ๋ฐ ์๊ฐ ์์ผ๋ฏ๋ก button์ ๋ณ๋๋ก ์์ฑํด์ input์ ๊พธ๋ฏผ ๊ฒ์ฒ๋ผ ๋ณด์ด๊ฒ ํ ๊ฒ์ด๋ค.  
input์ multiple ์์ฑ์ ๋ค์ํ ํ์ผ์ ๋ฑ๋กํ  ์ ์๊ฒ ๋ง๋ค์ด์ฃผ๊ณ , image/\* ๋ ์ด๋ฏธ์ง ํ์ผ์ ๋ชจ๋  ํ์ฅ์๋ฅผ ํ์ฉํ๋ค๋ ์๋ฏธ์ด๋ค.  
๋ง์ง๋ง Tweet ๋ฒํผ์ form ๋ด๋ถ์์ ์์ฑํ ๋ด์ฉ์ ์๋ฒ์ ์ ์ถํ๋ ๊ธฐ๋ฅ์ ํด์ผํ๋ฏ๋ก type์ submit์ผ๋ก ํ๋ค.

์ด๋ฒ์๋ ํ๋จ ๊ฒ์๋ฌผ์ธ ํ์๋ผ์ธ์ ๋ค์ด๊ฐ ๋ถ๋ถ์ ์ดํด๋ณด์.  
์ด ๋ถ๋ถ๋ ๋ง์ฐฌ๊ฐ์ง๋ก, ํ์๋ผ์ธ์ ๋ณด์ฌ์ฃผ๋ ๊ฒ์ ๋ผ๋ฆฌ์  ๊ตฌ๋ถ์ด ๋ชํํ๋ฏ๋ก **section** ํ๊ทธ๋ฅผ ์ฌ์ฉํ๋ค.

```html
<section>
  <h1>Your Timeline</h1>
  <ol>
    <li>
      <!--Tweet-->
    </li>
    <li>
      <!--Tweet-->
    </li>
    <li>
      <!--Tweet-->
    </li>
  </ol>
</section>
```

**section** ํ๊ทธ๋ sectioning tag์ด๋ฏ๋ก h ํ๊ทธ๋ฅผ ์ฌ์ฉํด์ ์ ๋ชฉ์ ์ ์ด์คฌ๋ค.  
ํ์๋ผ์ธ์ ์๊ฐ์ ๋ฐ๋ผ ์์๊ฐ ์์ผ๋ฏ๋ก **ol**์ ์ฌ์ฉํ๋ค.  
๊ฐ๊ฐ์ li์๋ ํด๋น ํ์๋ผ์ธ์ ๊ฒ์๋ฌผ์ด ๋ค์ด๊ฐ๋ฉด ๋  ๊ฒ์ด๋ค.  
๊ทธ๋ ๋ค๋ฉด ๊ฒ์๋ฌผ์ ๋งํฌ์ํ๋ ๊ฒ์ ์ดํด๋ณด์.

## ๐ article

**article**์ ๊ฒ์๋ฌผ๊ณผ ๊ฐ์ ์์๋ฅผ ์์ฑํ  ๋ ์ฌ์ฉํ๋ sectioning tag์ด๋ค.  
๋ฐ๋ผ์ ์ฌ์ฉ ํ h ํ๊ทธ๋ก ์ ๋ชฉ์ ์๋ ฅํด์ค์ผํ๋ค.  
์ฐ์ , ๊ฒ์๊ธ๋ header, ๋ด์ฉ, footer ๋ถ๋ถ์ผ๋ก ๋๋ ์ ์์ ๊ฒ ๊ฐ๋ค.  
header ๋ถ๋ถ๋ถํฐ ์ดํด๋ณด์.

```html
<article>
  <h1>A tweet from ๊น์ต๋ช</h1>
  <header>
    <a href="#">
      <img src="#" alt="๊น์ต๋ช" />
    </a>

    <h2>
      <a href="#">๊น์ต๋ช </a>
    </h2>

    <dl>
      <div>
        <dt>Username</dt>
        <dd>
          <a href="#"> @anonymouskim </a>
        </dd>
      </div>
      <div>
        <dt>Posted</dt>
        <dd>
          <a href="#"> Dec 25 </a>
        </dd>
      </div>
    </dl>

    <button type="button" aria-label="options">
      <!--icon-->
    </button>
    <!--Dropdown menu-->
    <div>
      <button type="button">
        <!--icon-->
        Show less often
      </button>
      <button type="button">
        <!--icon-->
        Embed Tweet
      </button>
      <button type="button">
        <!--icon-->
        Unfollow @anonymouskim
      </button>
      <button type="button">
        <!--icon-->
        Mute @anonymouskim
      </button>
      <button type="button">
        <!--icon-->
        Block @anonymouskim
      </button>
      <button type="button">
        <!--icon-->
        Report Tweet
      </button>
    </div>
  </header>
</article>
```

header ๋ถ๋ถ์๋ ํ๋กํ ์ด๋ฏธ์ง, ์ ์  ์ด๋ฆ, ์ ์  ๋๋ค์, ์์ฑ ๋ ์ง๊ฐ, ๊ทธ๋ฆฌ๊ณ  Dropdown menu๋ฅผ ํฌํจํ ๋ฒํผ์ด ์กด์ฌํ๋ค.  
์ ์  ์ด๋ฆ, ์ ์  ๋๋ค์, ์์ฑ ๋ ์ง์ ๊ฒฝ์ฐ dl๋ฅผ ์ฌ์ฉํด์ ์ด๋ค ํ์คํธ๊ฐ ์ด๋ค ์๋ฏธ๋ฅผ ๊ฐ์ง๊ณ  ์๋๊ฑด์ง ์ฝ๊ฒ ํ์ํด ์ค ์ ์์ ๊ฒ์ด๋ค.
Dropdown menu๋ ์์์๋ ์์ฃผ ๋์์ผ๋ฏ๋ก ์ค๋ช ์๋ต!

๊ฒ์๋ฌผ์ ๋ด์ฉ ๋ถ๋ถ์ p ํ๊ทธ๋ฅผ ํ์ฉํด์ ์์ฑํ๋ค.  
๋ง์ฝ ๋ณ๋๋ก ์ฌ์ง ๋ฑ์ ์๋ก๋ํ  ๊ฒฝ์ฐ์๋ ์ด ๋ถ๋ถ์ ์ฝ์ํ๋ฉด ๋  ๊ฒ์ด๋ค.

```html
<p>
  ์์ด๋ฅผ ๋ ์ ํ๊ณ ์ถ๋ค. ๊ทธ๋ฌ๋ ๊ณต๋ถ๋ฅผ ํ๊ณ  ์ถ์ง๋ ์๋ค. ๋ด ์ถ์ ๋ชจ๋  ๊ฒ์ด ์ด๋ฐ
  ์์ผ๋ก ๋งํด์๋ค
</p>
```

## ๐ footer

๋ค์์ผ๋ก๋ ๊ฒ์๋ฌผ์ ํ๋จ๋ถ์ ์๋ ๋๊ธ, ๋ฆฌํธ์, ์ข์์, ๊ณต์  ๋ฒํผ์ ์ดํด๋ณด์.  
์ด ๋ถ๋ถ์ ์์์ ํ ๋ฌถ์ ์ค ํ๋จ์ ์์นํ๋ฏ๋ก **footer**๋ฅผ ์ฌ์ฉํด์ ๋ฌถ์ด์ค๋ค.

```html
<article>
  <footer>
    <button type="button">
      <!--icon-->
      <span class="sr-only">Tweet your reply</span>
      <strong aria-label="3 replied">3</strong>
    </button>

    <button type="button">
      <!--icon-->
      <span>Retweet</span>
      <strong aria-label="3 retweeted">3</strong>
    </button>
    <!--Dropdown menu-->
    <div>
      <button type="button">Retweet</button>
      <button type="button">Retweet with comment</button>
    </div>

    <button type="button">
      <!--icon-->
      <span class="sr-only">Like this tweet</span>
      <strong aria-label="100 people liked">100</strong>
    </button>

    <button type="button">
      <!--icon-->
      <span class="sr-only">Share</span>
    </button>
    <!--Dropdown menu-->
    <div>
      <button type="button">Send via Direct Message</button>
      <button type="button">Add Tweet to Bookmarks</button>
      <button type="button">Copy link to Tweet</button>
    </div>
  </footer>
</article>
```

Dropdown menu๋ ๋ชจ๋ฌ ์ฐฝ์ผ๋ก ๋ณด์ฌ์ฃผ๋ ๋ฉ๋ด๊ฐ ํ ํ์ด์ง์์๋ ๊ต์ฅํ ์์ฃผ ๋์ค๋ ๊ฒ์ ์ ์ ์๋ค.  
๋ฐ๋ณต์ ์ธ ์ค๋ช์ด๋ฏ๋ก ์๋ต!

## ๐ aside

์ด๋ฒ์๋ ์น ํ์ด์ง์ ์์ ๋ณด์ด๋ ๋ถ๊ฐ์ ์ธ ์์๋ค์ ๋ํด์ ์์๋ณด์.  
์ด๋ค์ **aside** ํ๊ทธ๋ฅผ ์ฌ์ฉํ์ฌ ๋ฌถ์ด์ค๋ค.  
Who to follow ๋ถ๋ถ์ ์๋ตํ๋๋ก ํ๊ฒ ๋ค.

<img width="392" alt="แแณแแณแแตแซแแฃแบ 2022-02-25 แแฉแแฅแซ 11 39 19" src="https://user-images.githubusercontent.com/86224851/155643353-eed1e960-d797-4bd7-ba75-c141cf882bdb.png">

Search Twitter ๋ถ๋ถ์ ์๋ตํ๋๋ก ํ๊ฒ ๋ค.  
Worldwide trends ๋ถ๋ถ์ ์์์๋ ๋ง์ด ๋ค๋ฃฌ ํํ์ด๋ค.  
ํ๋์ ์ ๋ชฉ๊ณผ Dropdown menu๊ฐ ๋๊ฒ ๋ค.  
์ด๋ค์ header๋ก ๊ฐ์ธ ๋จธ๋ฆฌ ๋ถ๋ถ์์ ์๋ ค์ฃผ์.

```html
<aside>
  <header>
    <h1>Worldwide Trends</h1>
    <button type="button" aria-label="options">
      <!--icon-->
    </button>
    <!--Dropdown menu-->
  </header>
</aside>
```

๊ทธ ๋ค์์ผ๋ก๋ Worldwide trend๋ฅผ ์ง์ ์ ์ผ๋ก ํ์ํ๋ ๋ถ๋ถ์ด๋ค.  
์์๊ฐ ์ค์ํ๋ฏ๋ก **ol**์ ์ฌ์ฉํ์.
๊ฐ๊ฐ์ li ์์๋ ์ถ๊ฐ์ ์ธ ์์๊ฐ ์๋ค.

```html
<aside>
  <ol>
    <li>
      <a href="#">
        <span>1 โข Trending worldwide</span>
        <strong lang="ko">#๊น๋ฒ๊ทธ</strong>
        <span>100K Tweets</span>
      </a>

      <button type="button" aria-label="options">
        <!--icon-->
      </button>
      <div>
        <button type="button">
          <!--icon-->
          This trend is spam
        </button>
        <button type="button">
          <!--icon-->
          This trend is spam
        </button>
        <button type="button">
          <!--icon-->
          This trend is spam
        </button>
        <button type="button">
          <!--icon-->
          This trend is spam
        </button>
        <button type="button">
          <!--icon-->
          This trend is spam
        </button>
      </div>
    </li>
  </ol>
  <button type="button">Show more</button>
</aside>
```

์ธ๋ถ์ ์ธ ๋ถ๋ถ๋ ํ์คํธ์ Dropdown menu์ ์กฐํฉ์ด๋ฏ๋ก ์ค๋ช์ ์๋ตํ๊ฒ ๋ค!  
๋ง์ง๋ง ๋ถ๋ถ์๋ ๊ฐ๋ ค์ง ๋ฆฌ์คํธ๋ฅผ ๋ณด์ฌ์ฃผ๋ ๊ธฐ๋ฅ์ ํ๋ button์ด ์๋ค.

<img width="313" alt="แแณแแณแแตแซแแฃแบ 2022-02-25 แแฉแแฅแซ 11 59 19" src="https://user-images.githubusercontent.com/86224851/155645432-11f6f920-706b-4c95-acf5-0c718912ce0f.png">

๋ง์ง๋ง์ผ๋ก ํ์ฌ๋ช, ์ถ๊ฐ ๋ฉ๋ด, ์ ์๊ถ ๋ฑ์ด ๋ค์ด๊ฐ๋ ์น ํ์ด์ง ์ ์ฒด์ ํ๋จ๋ถ๋ฅผ ์ดํด๋ณด์.  
์ด๋ฏธ ์์ ์ด๋ฐ ๋ถ๋ถ์ **footer**๋ฅผ ์ฌ์ฉํ๋ค๋ ๊ฒ์ ์๊ณ ์๋ค.

```html
<footer>
  <a href="#" target="_blank">Terms</a>
  <a href="#" target="_blank">Privacy policy</a>
  <a href="#" target="_blank">Cookies</a>
  <a href="#" target="_blank">Ads info</a>

  <button type="button">
    More
    <!--icon-->
  </button>
  <!--Dropdown menu-->
  <div>
    <a href="#" target="_blank">About</a>
    <a href="#" target="_blank">Status</a>
    <a href="#" target="_blank">Businesses</a>
    <a href="#" target="_blank">Developers</a>
  </div>

  <span>ยฉ 2019 Twitter, Inc.</span>
</footer>
```

์ด ๋ถ๋ถ๋ ์ฌ์ค ๋์ฌ๊ฒจ๋ณผ๋งํ ๊ณณ์ ์๋ค.  
ํ๋ ํ์คํ๊ฑด ํน์  ๊ตฌ์กฐ๊ฐ ์ฝ๊ฐ์ ๋ณํ์ผ๋ก ๊ณ์ ๋ฐ๋ณต๋๋ค๋ ๊ฒ์ด๋ค.  
๋ฌผ๋ก  ํธ์ํฐ๋ง ๊ทธ๋ด ์๋ ์์ง๋ง...  
์ด๋ค ํ๊ทธ๋ฅผ ์ด๋ค ์ํฉ์ ์ฌ์ฉํด์ํ ์ง ๊ฐ์ด ์กํ๋ ๊ฒ ๊ฐ๋ค!

๐ฅณ ์๊ณ ํ์จ์ต๋๋ค~
