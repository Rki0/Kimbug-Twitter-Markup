# 🕊 Twitter Markup (HTML sectioning tag)

<img src="https://user-images.githubusercontent.com/86224851/155629398-5b5bd475-310a-4d67-a36f-469c6ef2f29c.jpeg">

트위터 홈페이지의 HTML 문서를 작성할 때 어떤 식으로 구획을 나누고 각각의 요소들을 구현하는지에 대해서 살펴보면서, HTML sectioning tag에 대해 공부하자.  
HTML에 구획에 대한 공부이므로 CSS와 JS는 언급하지않는다.

기본적으로 알고 가야할 것이 있다.  
sectioning tag에는 section, article, nav, aside가 있다.  
이들은 사용 후 반드시 heading 태그(h 태그)를 사용해서 제목을 표시해줘야한다.  
그게 사용자에게 보이는 부분이든 아니든 꼭!

## 😉 header

<img width="483" alt="스크린샷 2022-02-25 오전 9 30 48" src="https://user-images.githubusercontent.com/86224851/155630602-960cb2da-8192-4346-b9e4-1b78222d3fe2.png">

보통 일반적인 사이트의 경우 회사 로고와 메뉴바가 위쪽에 있어 header로 생각하기 편한데, 트위터의 경우 세로로 분할되어 있어 약간 신선하다.  
형태만 달라졌을 뿐이므로 붉은색 표시 부분을 **header**로 묶어주겠다.

로고 부분과 메뉴바 부분은 해당 페이지로 이동하거나 추가 메뉴를 보여주는 등 기능은 비슷하다.  
하지만 로고의 경우 페이지를 대표하는 느낌이 있으므로 따로 작성하는 것으로 하자.

```html
<header>
  <!--회사 로고-->
  <h1>
    <a href="#">
      <img src="#" alt="Twitter" />
    </a>
  </h1>
</header>
```

h1 태그를 사용해서 대표성을 강조해줬고, 로고 이미지를 클릭하면 홈페이지로 이동하므로 a 태그로 감싸주었다.

## 😉 nav

다음으로는 메뉴바를 만들 것이다.  
문서 페이지 간 이동하는 것이 있는 경우 **nav** 태그를 사용한다.

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

**nav**는 sectioning tag이므로 사용 후 heading 태그를 사용하여 제목을 달아줬다.  
메뉴바에 들어갈 요소들은 순서없이 나열된 리스트이므로 **ul**을 사용하여, 각각을 **li**로 만들어줬다.  
ul은 직계 자손으로 li만을 받으므로 a 태그를 사용하고 싶다면 li 안에 작성해야한다.  
Home 메뉴에는 span을 사용해서 이 부분이 어떤 의미를 가지고 있는지 설명을 작성했다. span은 얼마든지 CSS로 지울 수 있으니...  
Notifications라는 메뉴에는 5개의 새로운 알람이 있다는 표시가 있는데, 이는 사용자에게 강조해야할 부분이므로 **strong**을 사용해서 표시해줬다.  
More 메뉴는 클릭 시 Dropdown menu가 생성된다. 따라서 a가 아닌 button 태그를 사용한다.

## 😉 main

main 태그는 html 문서에서 단 한번만 사용 가능한 태그로, 웹 페이지의 주된 내용이 보여질 부분이다.

<img width="621" alt="스크린샷 2022-02-25 오전 10 01 02" src="https://user-images.githubusercontent.com/86224851/155633566-876b6baf-4930-4715-ba07-fdf216409c2c.png">

붉은 색으로 표시해놓은 부분은 상단에 나의 트윗을 적는 곳과 하단에 게시물들이 보인다.  
사용자가 주로 사용하는 부분이므로 이를 **main** 태그로 묶어주도록 하겠다.  
우선, Home 표시가 있는 부분을 살펴보자.  
Home이라는 제목과 어떤 버튼이 있다.  
이 버튼은 클릭 시 Dropdown menu가 나온다.

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
        <span> 올라오는 순서대로 트윗이 표시됩니다. </span>
      </button>
      <a href="#">
        <!--icon-->
        콘텐츠 환경설정 보기
      </a>
    </div>
  </header>
</main>
```

main 중에서도 윗부분에 존재하므로 header를 사용해서 작성했다.
button을 클릭 시 보여줄 Dropdown menu를 div를 활용해 별도로 묶어놓은 것을 볼 수 있다.

## 😉 section

다음으로는 나의 트윗을 작성하는 곳을 살펴보자.  
이 부분은 텍스트를 작성하는 곳으로 그 논리적인 구분이 명확하게 다른 곳과 구별될 수 있으므로 **section**을 통해 구획을 묶어주었다.

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

**section** 태그는 sectioning tag이므로 h 태그를 사용해서 제목을 적어줬다.  
트윗을 작성하는 부분을 보면 이미지와 텍스트 입력부, 각종 기능의 버튼이 있다.  
이들은 각각이 연결되어 있는 동작을 하므로 하나의 form 태그 안에 넣어주는 것이 좋을 것 같다.  
하단에 다양한 기능을 하는 버튼들이 보인다.  
설명은 "button"이라고 하지만 실제 파일을 삽입하는 등의 기능은 "input"을 통해 구현한다.  
문제는 input 태그는 꾸밀 수가 없으므로 button을 별도로 생성해서 input을 꾸민 것처럼 보이게 한 것이다.  
input의 multiple 속성은 다양한 파일을 등록할 수 있게 만들어주고, image/\* 는 이미지 파일의 모든 확장자를 허용한다는 의미이다.  
마지막 Tweet 버튼은 form 내부에서 작성한 내용을 서버에 제출하는 기능을 해야하므로 type을 submit으로 했다.

이번에는 하단 게시물인 타임라인에 들어갈 부분을 살펴보자.  
이 부분도 마찬가지로, 타임라인을 보여주는 것은 논리적 구분이 명확하므로 **section** 태그를 사용한다.

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

**section** 태그는 sectioning tag이므로 h 태그를 사용해서 제목을 적어줬다.  
타임라인은 시간에 따라 순서가 있으므로 **ol**을 사용한다.  
각각의 li에는 해당 타임라인의 게시물이 들어가면 될 것이다.  
그렇다면 게시물을 마크업하는 것을 살펴보자.

## 😉 article

**article**은 게시물과 같은 요소를 작성할 때 사용하는 sectioning tag이다.  
따라서 사용 후 h 태그로 제목을 입력해줘야한다.  
우선, 게시글도 header, 내용, footer 부분으로 나눌 수 있을 것 같다.  
header 부분부터 살펴보자.

```html
<article>
  <h1>A tweet from 김익명</h1>
  <header>
    <a href="#">
      <img src="#" alt="김익명" />
    </a>

    <h2>
      <a href="#">김익명 </a>
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

header 부분에는 프로필 이미지, 유저 이름, 유저 닉네임, 작성 날짜가, 그리고 Dropdown menu를 포함한 버튼이 존재한다.  
유저 이름, 유저 닉네임, 작성 날짜의 경우 dl를 사용해서 어떤 텍스트가 어떤 의미를 가지고 있는건지 쉽게 표시해 줄 수 있을 것이다.
Dropdown menu는 위에서도 자주 나왔으므로 설명 생략!

게시물의 내용 부분은 p 태그를 활용해서 작성했다.  
만약 별도로 사진 등을 업로드할 경우에는 이 부분에 삽입하면 될 것이다.

```html
<p>
  영어를 더 잘 하고싶다. 그러나 공부를 하고 싶지는 않다. 내 삶의 모든 것이 이런
  식으로 망해왔다
</p>
```

## 😉 footer

다음으로는 게시물의 하단부에 있는 댓글, 리트윗, 좋아요, 공유 버튼을 살펴보자.  
이 부분은 요소의 한 묶음 중 하단에 위치하므로 **footer**를 사용해서 묶어준다.

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

Dropdown menu나 모달 창으로 보여주는 메뉴가 한 페이지에서도 굉장히 자주 나오는 것을 알 수 있다.  
반복적인 설명이므로 생략!

## 😉 aside

이번에는 웹 페이지의 옆에 보이는 부가적인 요소들에 대해서 알아보자.  
이들은 **aside** 태그를 사용하여 묶어준다.  
Who to follow 부분은 생략하도록 하겠다.

<img width="392" alt="스크린샷 2022-02-25 오전 11 39 19" src="https://user-images.githubusercontent.com/86224851/155643353-eed1e960-d797-4bd7-ba75-c141cf882bdb.png">

Search Twitter 부분은 생략하도록 하겠다.  
Worldwide trends 부분은 위에서도 많이 다룬 형태이다.  
하나의 제목과 Dropdown menu가 되겠다.  
이들은 header로 감싸 머리 부분임을 알려주자.

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

그 다음으로는 Worldwide trend를 직접적으로 표시하는 부분이다.  
순서가 중요하므로 **ol**을 사용하자.
각각의 li 안에도 추가적인 요소가 있다.

```html
<aside>
  <ol>
    <li>
      <a href="#">
        <span>1 • Trending worldwide</span>
        <strong lang="ko">#김버그</strong>
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

세부적인 부분도 텍스트와 Dropdown menu의 조합이므로 설명을 생략하겠다!  
마지막 부분에는 가려진 리스트를 보여주는 기능을 하는 button이 있다.

<img width="313" alt="스크린샷 2022-02-25 오전 11 59 19" src="https://user-images.githubusercontent.com/86224851/155645432-11f6f920-706b-4c95-acf5-0c718912ce0f.png">

마지막으로 회사명, 추가 메뉴, 저작권 등이 들어가는 웹 페이지 전체의 하단부를 살펴보자.  
이미 앞서 이런 부분은 **footer**를 사용한다는 것을 알고있다.

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

  <span>© 2019 Twitter, Inc.</span>
</footer>
```

이 부분도 사실 눈여겨볼만한 곳은 없다.  
하나 확실한건 특정 구조가 약간의 변형으로 계속 반복된다는 것이다.  
물론 트위터만 그럴 수도 있지만...  
어떤 태그를 어떤 상황에 사용해아할지 감이 잡히는 것 같다!

🥳 수고하셨습니다~
