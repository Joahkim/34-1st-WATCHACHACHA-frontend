#  Watcha Classic
- Front: 김민석, 김은경, 이현범
- Back: 이태권, 박민하
![image](https://user-images.githubusercontent.com/50426259/176836350-67dbc6fa-eee8-4f0e-b675-d9da0865a350.png)
[시현 영상 보러가기](https://scrawny-opera-4c6.notion.site/ded2dbffac2140609d15bc3877219332)

<br>

## 프로젝트 소개
SNS와 평정 데이터를 활용한 클래식 영화 백과사전 사이트

<br>

## 사용기술 스택
## 사용기술 스택
- Front-end: <img src="https://img.shields.io/badge/html5-E34F26?style=flat-square&logo=html5&logoColor=white"/> <img src="https://img.shields.io/badge/Sass-CC6699?style=flat-square&logo=Sass&logoColor=white"/> <img src="https://img.shields.io/badge/javascript-F7DF1E?style=flat-square&logo=javascript&logoColor=white"/> <img src="https://img.shields.io/badge/react-61DAFB?style=flat-square&logo=react&logoColor=white"/> <img src="https://img.shields.io/badge/ReactRouter-CA4245?style=flat-square&logo=ReactRouter&logoColor=white"/>
- Back-end: <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=Python&logoColor=white"/> <img src="https://img.shields.io/badge/Django-092E20?style=flat-square&logo=Django&logoColor=white"/> <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=MySQL&logoColor=white"/>

<br>

## Front-end 필수구현 기능
> ### 1. 회원가입 / 로그인 페이지
  - 유효성 검사, back-end API 통신
  - Nav 버튼 클릭 시 로그인 / 회원가입 모달창 오픈

> ### 2. 메인 페이지
  - 라이브러리 없이 이미지 슬라이드 구현
  - 3개의 API 한 페이지에 받아오기
  - Advanced Router 사용하여 각각의 목록 클릭시 path parameter id 값 불러오기

> ### 3. 상세 페이지
  - 스켈레톤, 평가 별점, 보고싶어요 댓글 UI 구현
  - <보고싶어요> 버튼 클릭 시 보고싶어요 페이지로 데이터 전송

> ### 4. 프로필 페이지
  - 회원정보 보여주기
  - <보고싶어요> 담긴 갯수 보여주기 
 
> ### 5. 보고싶어요 페이지
  - 메인 페이지의 컴포넌트 재사용
  - 사용자가 보고싶어요 기능 사용한 데이터 받아오기

<br>

## 소통에 사용한 협업 툴
### Slack
<img width="942" alt="스크린샷 2022-07-01 오후 3 48 13" src="https://user-images.githubusercontent.com/50426259/176840075-30907e6a-8be6-4914-88d3-fe0d3742ad9c.png">

- Back-end와 자료 공유 및 개인적인 소통

### Trello
![trello](https://user-images.githubusercontent.com/50426259/176840626-5bc5b445-4c0b-4259-93bd-56d9f63f2485.gif)
- 미팅에서 각자의 작업 현황 공유

### Notion
![image](https://user-images.githubusercontent.com/50426259/176840968-aab75ef3-4a5c-4497-a532-db539a297b58.png)
- 매일 진행되는 Stand-up meeting에서 각자의 진행 상황과 블로커 파악 및 소통

### ERD
![image](https://user-images.githubusercontent.com/50426259/176841194-db70fa46-6f62-4a65-8638-3c2562092a32.png)
- Back-end의 ERD 자료 구성을 참고하여 Mockdata 및 실제 서버와 통신시 불러오는 key값 확인

<br>

---


<br>

# 개인이 담당했던 page 상세 설명
## :: 최근 작업 주제 (하나 이상의 주제를 선택해주세요.)
- [x] 기능 추가 
- [ ] 리뷰 반영
- [ ] 리팩토링
- [ ] 버그 수정
- [ ] 컨벤션 수정
<br>

### :: 매일 기록하기
- [x] 초기 세팅 완료 후 branch 생성
- [x] 6/21 mainPage branch에서 레이아웃 구성 완료
- [x] 6/22 mainPage Mock Data 생성하여 map 함수 사용하기 
- [x] 6/22 mainPage 슬라이드 구현 (진행중)
- [x] 6/23 [First] 리뷰반영 수정사항 기록
- [x] 6/24 슬라이드 구현 완료, MockData 수정 
- [x] 6/27 서버에서 <영화목록> 데이터 받아오기 
- [x] 6/28 mainPage 구현 완료 

<br />

## :: 구현 목표 (해당 브랜치에서 구현하고자 하는 하나의 목표를 설정합니다.)
- 초기 세팅 완료
- <영화목록> 컴포넌트 생성 
- <Mock data 생성> 해당 데이터로 map함수 실행
- <mainPage 슬라이드> translate-X로 px에 따라 이동하기 구현
- 6/23 [First] 리뷰반영 수정사항
- 6/24 슬라이드 완료
- 6/27 서버에서 영화목록 일부 데이터 받아오기 성공
- 6/28 메인 페이지 구현 완료(리팩토링)

<br />

## :: 구현 사항 설명 (작업한 내용을 상세하게 기록합니다.)

#### 1. 초기 세팅 완료 후 branch 생성

#### 2. <영화목록> 컴포넌트 생성
![image](https://user-images.githubusercontent.com/50426259/174825313-5d610984-78c9-4379-94fd-7c2e721a1932.png)
총 세번 반복되는 '영화 목록' `<ul className="filmList">` 태그로 작성한다.
`<ul>`태그 안에는 각 영화들의 포스터와 간략한 정보를 나타내는 10개의 영화`<li className="firstLow">`

```javascript
    <ul className="filmList">
      <FirstLow />
      <FirstLow />
      <FirstLow />
      <FirstLow />
      <FirstLow />
      <FirstLow />
      <FirstLow />
      <FirstLow />
      <FirstLow />
      <FirstLow />
    </ul>
```
(아직 Mock Data 구현 전 해당 컴포넌트를 10개 작성하였다. 내일 mock data를 구현해야 한다.)
<br>

해당 `<FirstLow/>` 영화 포스터를 나타낼 수 있는 `<div className="posterBox">` 안에 `<img>`로 이미지를 불러온다.영화의 기본적인 정보를 나타내는 박스를 같은 부모 안에 형제 요소로 생성한다. `<div className="filmDescription">`
컴포넌트 안에는 각각의 영화를 클릭하면 상세페이지로 이동할 수 있게 `<Link/>` `<li>` 태그 안에 묶이는 모든 내용을 포함한다. 따라서 영화 포스터 이미지, 영화 이름, 영화 개봉일 등의 텍스트를 클릭해도 해당 영화의 상세 페이지인 `details`로 이동할 수 있게 설정했다.
```javascript
<li className="firstLow">
  <Link to="/details" className="film1Detail">
    <div className="posterBox">
      <img
        src="/images/poster/TheGreatGatsby.jpg"
        alt="개츠비"
        className="filmPosters"
      />
    </div>
    <div className="filmDescription">
      <p className="filmName">위대한 개츠비</p>
      <p className="filmYear">1920 ▪ 미국</p>
      <p className="filmAverage">평균★3.7</p>
    </div>
  </Link>
</li>
```
<br />

#### 3. <Mock Data> 생성과 데이터를 활용하여 <영화목록> map 함수 적용하기
백엔드와 소통 후 Mock Data를 대략적으로 구성했다.  아직 정확한 테이블이 나오지 않아서 다소 백엔드의 테이블과 상이 하지만 내가 `fetch`함수를 작성해서 데이터를 불러오는데에 문제가 없이 작성했다.
- `name`에는 영화 이름이 들어가야 하는데 일단은 팀원들 이름으로 작성
- 제작 국가의 카테고리가 생각보다 복잡해서 일단은 보류하고 하드코딩으로 남겨두었다.

```javascript
[
  {
    "id": 1,
    "name": "이태권",
    "release_date": 1920,
    "image_url": "/images/poster/TheGreatGatsby.jpg",
    "films_countries": {
      "countries": "미국"
    }
  },
  {
    "id": 2,
    "name": "김민석",
    "release_date": 1920,
    "image_url": "/images/poster/TheGreatGatsby.jpg"
  },
  {
    "id": 3,
    "name": "김은경",
    "release_date": 1920,
    "image_url": "/images/poster/TheGreatGatsby.jpg"
  }
]
```
<br>

- `fetch`함수로 Mock data 가져오기

```javascript
const [movies, setMovies] = useState([]);
useEffect(() => {
  fetch("/data/mainMock.json")
    .then(res => res.json())
    .then(data => {
      setMovies(data);
    });
}, []);
```
- Mock data에서 가져온 데이터를 movies에 할당하여 사용한다.

```javascript
<ul className="filmList">
  {movies.map(movie => (
    <FirstLow
      slide={slidePx}
      key={movie.id}
      id={movie.id}
      name={movie.name}
      date={movie.release_date}
      url={movie.image_url}
    />
  ))}
</ul>
```

- 해당 데이터를 MainBox.js 작성하여 데이터의 value값을 FirstLow 컴포넌트에 넘겨준다.

#### 3-1. `<ul>` 태그까지 포함하여 새로운 컴포넌트 만들기
해당 컴포넌트는 `<MainBox/>`이며 내부에는 `<FilmList/>` 컴포넌트가 포함되어 있다.

```javascript
<div className="mainWrapper">
  <MainBox movies={movies} />
  <MainBox movies={movies} />
  <MainBox movies={movies} />
</div>
```
- `<MainBox/>`는 3번 사용될 것이다. 아직 수정할 부분이 많다. 영화 목록 테마 같은 경우는 1970, 1960, 1980 년대와 같이 목록이름이 달라야 한다. 이 부분은 추후에 Mock Data 수정과 함께 변경하자.

```javascript
//MainBox.js

<div className="mainBox1">
  <p className="filmTheme1">1970's Films</p>
  <ul className="filmList">
    {movies.map(movie => (
      <FirstLow
        slide={slidePx}
        key={movie.id}
        id={movie.id}
        name={movie.name}
        date={movie.release_date}
        url={movie.image_url}
      />
    ))}
  </ul>
  <div
    className="prevBtn"
    onClick={toPrev}
    style={{ display: `${btnShow}` }}
  >
    <i className="fa-solid fa-chevron-left" />
  </div>
  <div
    className="nextBtn"
    onClick={toNext}
    style={{ display: `${!btnShow}` }}
  >
    <i className="fa-solid fa-chevron-right" />
  </div>
</div>
```

#### 3-2. 슬라이드 구현하기

```javascript
//우선 인라인 스타일을 부여했다.
// FilmList.js
<li
  className="firstLow"
  id={id}
  style={{
    transform: `translateX(${slide}px)`,
    transition: "0.5s ease",
  }}
>
  <Link to="/details" className="film1Detail">
    <div className="posterBox">
      <img src={url} alt="개츠비" className="filmPosters" />
    </div>
    <div className="filmDescription">
      <p className="filmName">{name}</p>
      <p className="filmYear">{date} ▪ 미국</p>
      <p className="filmAverage">평균★3.7</p>
    </div>
  </Link>
</li>
```

- `<FilmList/>`컴포넌트가 초기 화면에서 5개가 보여지는데 버튼을 클릭하면 5개의 크기만큼 왼쪽으로 이동한다.
- translate-X 값을 5개 크기인 1375px 만큼 부여한다. 
- `nextBtn`을 클릭하면 x축으로 -1375px 움직인다.
- `prevBtn`은 반대로 1375px 만큼 움직인다.
- 처음 화면에서 `preBtn`은 보이지 않는다. (왼쪽으로는 컨텐츠가 없기 때문)
- `nextBtn`을 한 번이라도 클릭하여 영화 목록들이 이동을 하면 생성된다.(display : block or none)

```javascript
  const [slidePx, setSlidePx] = useState(0);
  const [btnShow, setBtnShow] = useState("none");
  const toPrev = () => {
    if (slidePx < -1374) {
      setSlidePx(slidePx + 1375);
    } else {
      setBtnShow("none");
    }
  };
  const toNext = () => {
    if (slidePx > -1376) {
      setSlidePx(slidePx - 1375);
      setBtnShow("");
    }
```
#### 4. [First] 리뷰 반영 코드 수정
#### 4-1 import 순서, 줄바꿈, CSS 속성 순서, 중복되는 width값 불필요한 값 삭제 등 스타일링에 관련된 수정 요청

#### 4-2 `props`를 한 번에 넘겨주기 => 가독성 높이기 위함
>이전 코드

```javascript
//MainBox.js

<ul className="filmList">
  {movies.map(movie => (
    <Film slide={slidePx} 
      key={movie.id} 
      id={movie.id}
      name={movie.name} 
      date={movie.release_date} 
      url={movie.image_url} />
  ))}
</ul>

//Film.js

const Film = ({ slide,  id, name, date, url }) => {
  return (
    <li
      className="film"
      key={id}
      style={{
        transform: `translateX(${slide}px)`,
        transition: "0.5s ease",
      }}
    >
      <Link to="/details" className="filmDetail">
        <div className="posterBox">
          <img src={url} alt="개츠비" className="filmPosters" />
        </div>
        <div className="filmDescription">
          <p className="filmName">{name}</p>
          <p className="filmYear">{date} ▪ 미국</p>
          <p className="filmAverage">평균★3.7</p>
        </div>
      </Link>
    </li>
  );
};
```
** 위의 코드를 수정해야 하는 이유? 가독성이 좋지 않은 이유? **
- MainBox.js 에서 데이터를 풀어서 Film.js에 넘겨주기 보다는 아직 데이터를 풀지 않고 Film.js에 넘겨주고 거기서 풀면 된다.
- 대신 구조분해 할당을 통해서! 객체를 구조분해 할당하려면 대괄호가 아닌 중괄호! 객체니깐!

> 수정 후 코드

```javascript
//MainBox.js

<div className="mainBox">
  <p className="filmTheme">1970's Films</p>
  <ul className="filmList">
    {movies.map(movie => (
      <Film slide={slidePx} key={movie.id} movie={movie} />
    ))}
  </ul>
``` 
- `movie` 안에 있는 데이터를 풀지 않고 그대로 `<Film>` 컴포넌트에 넘겨준다.

```javascript
const Film = ({ movie, slide }) => {
  const { id, name, release_date, image_url } = movie;
  return (
    <li
      className="film"
      id={id}
      style={{
        transform: `translateX(${slide}px)`,
        transition: "0.5s ease",
      }}
    >
      <Link to="/details" className="filmDetail">
        <div className="posterBox">
          <img src={image_url} alt="개츠비" className="filmPosters" />
        </div>
        <div className="filmDescription">
          <p className="filmName">{name}</p>
          <p className="filmYear">{release_date} ▪ 미국</p>
          <p className="filmAverage">평균★3.7</p>
        </div>
      </Link>
    </li>
  );
};
```
- `const { name, release_date, image_url } = movie;` 구조 분해할당을 `Film.js`에서 진행
- 위의 한 줄로 이전 MainBox.js에 작성했던 코드 세줄을 줄일 수 있다. 정리도 더 잘되는게 필요한 곳에서 `movie`를 풀어주는게 직관적이다. 

> 수정 과정 중 만났던 에러!
`map`함수를 작성하면 반드시 최상위 태그에 `key`를 작성해야 한다. 하지만 이 `key`는 <Films/>에 넘겨줄 수 없다.
마치 예약어처럼 `key`는 `map`함수를 사용할 때 따라다니는 속성이다. 우리는 `key` 속성을 함부로 넘겨줄 수 없다.
`key`는 부여만 가능하다.
Film.js에 `key`를 넘겨주었더니 "key is not a props" 라는 에러를 만났다.
이때 `key`를  `const { key, name, release_date, image_url } = movie;` 구조분해 할당으로 <Film/>에 넘겨주었기 때문이다.
앞으로 `key`는 그 존재만으로 역할을 할 뿐이라고 생각하자

#### 5. 슬라이드 구현 완료
- if문으로 px을 통해 슬라이드를 구현한다.
- 버튼을 클릭하면 콘텐츠의 길이(1375px)만큼 이동한다.

```js
  const [slidePx, setSlidePx] = useState(0);

  const toPrev = () => {
    slidePx < 0 && setSlidePx(slidePx + 1375);
  };

  const toNext = () => {
    slidePx > -2750 && setSlidePx(slidePx - 1375);
  };
```
- 우선 버튼을 눌렀을 때 어떤 기능을 해야하는지 생각한다. (단계적으로 생각하기)
- `prevBtn`은 초기 화면에서는 비활성화 되어 있어야 하기 때문에 `slidePx`이 0일 때는 클릭이 되면 안된다.
- 따라서, `slidePx`이 0보다 작을 때(음수)만 작동이 되어야 한다.
- 똑같은 원리로 `nextBtn`은 더 이상 보여줄 콘텐츠가 없을 때 비활성화 되어야 한다. 그때의 `slidePx`이 -2570값 보다 작다(음수니깐 >)

```js
<div className="prevBtn" onClick={toPrev} style={{ display: slidePx === 0 ? "none" : "" }}>
  <i className="fa-solid fa-chevron-left" />
</div>
<div className="nextBtn"  onClick={toNext} style={{ display: slidePx === -2750 ? "none" : "" }}>
  <i className="fa-solid fa-chevron-right" />
</div>
```
- 각각의 버튼의 비활성화를 위해 버튼에 인라인 스타일을 적용한다. 
- 삼항 연산자로 `slidePx`이 어떨때 버튼을 비활성화 해야하는지 조건을 작성한다.
- "block"도 가능하지만 빈 문자열을 부여하는 것과 동일하다.

#### 5-2. MockData 수정
![image](https://user-images.githubusercontent.com/50426259/175545650-d2508efa-281a-41ce-9208-22b3d973c176.png)

- 하드코딩으로 작성했던 부분을 MockData에 추가하여 `props` 값을 추가했다.

```js
  {
    "id": 1,
    "name": "개개",
    "release_date": 1920,
    "image_url": "/images/poster/copyrightfree.jpg",
    //추가한 데이터
     "country": "한국",
    //추가한 데이터
    "rate_stars": "평균★3.5"
  },
```
#### 6. 서버에서 영화목록 데이터 일부 받아오기
- 사용한 메소드 : fetch
- 새로운 개념 활용: Query parameter, Path parameter
![image](https://user-images.githubusercontent.com/50426259/175962281-e93214c9-6166-4e1b-82c2-6b16304ec307.png)


```js
//Main.js

const Main = () => {
  const [movies, setMovies] = useState([]);

  useEffect(() => {
    fetch("http://10.58.2.194:8000/films/main?genre=드라마")
      .then(res => res.json())
      .then(data => {
        setMovies(data);
      });
  }, []);

  if (movies.length === 0) return;

  return (
    <>
      <div>
        <h1 className="fakeNav">안녕하세요</h1>
      </div>
      <div className="mainWrapper">
        <MainBox movies={movies.results} theme={MOVIE_TITLE[0]} />
      </div>
    </>
  );
};

export default Main;
```
- 우선 백엔드에서 넘겨준 Query parameter를 사용한 주소를 `fetch` 함수에 작성한다.
- 백엔드에서 작성한 데이터는 객체 안에 results는 key가 value를 가지고 있었기 때문에 `movies.results`로 접근한다.

```js
//Router.js

const Routers = () => {
  return (
    <BrowserRouter>
      <Nav />
      <Routes>
        <Route path="/" element={<Main />} />
        <Route path="/detail/:id" element={<Detail />} />
      </Routes>
      <Footer />
    </BrowserRouter>
  );
};

export default Routers;
```
- 넘겨 받은 데이터 안에는 각 영화에 담긴 id 값을 가지고 있다.
- `피그말리온->{id: 14}` 해당 id 값을 Path parameter를 사용하여 `detail`페이지의 엔드포인트 뒤에 id 값으로 지정해야 한다.

```js
const Film = ({ movie, slide }) => {
  const { id, name, release_date, image_url, country, running_time_min } = movie;

  return (
    <li
      className="film"
      id={id}
      style={{
        transform: `translateX(${slide}px)`,
        transition: "0.5s ease",
      }}
    >
      <Link to={`/detail/${id}`} className="filmDetail">
        <div className="posterBox">
          <img src={image_url} alt="개츠비" className="filmPosters" />
        </div>
        <div className="filmDescription">
          <p className="filmName">{name}</p>
          <p className="filmYear">
            {release_date} • {country}
          </p>
          <p className="filmAverage">⏱️{running_time_min}분</p>
        </div>
      </Link>
    </li>
  );
};

export default Film;
```
- `<Link to={`/detail/${id}`} className="filmDetail">`로 각각의 영화목록을 클릭했을 때, 이동하는 링크를 Path parameter의 id를 매개변수로 작성하면 백에서 넘겨준 영화의 id값이 엔드 포인트 뒤에 붙으며 해당 영화의 상세페이지로 이동한다.

#### 7. mainPage 구현 완료
- 백엔드에서 계획을 변경했다. 원래는 3개의 API를 넘겨주고 프런트는 3개의 fetch함수를 사용하여 각각의 데이터를 각각의 useState를 사용하여 자식 컴포넌트에 넘겨준다.
- 하지만 시간문제 상 1개의 API에 모든 정보를 담아서 (내가 작성한 MockData와 동일한 형식) 하나의 fetch 함수로 받아와 각각의 MainBox 컴포넌트에 다른 정보를 넘겨준다.

```js
import React, { useEffect, useState } from "react";
import MainBox from "./components/MainBox/MainBox";
import "./Main.scss";

const Main = () => {
  const [movies, setMovies] = useState([]);

  useEffect(() => {
    fetch("http://172.20.10.11:8000/films?genre=드라마&country=미국&time=100")
      .then(res => res.json())
      .then(data => {
        setMovies(data);
      });
  }, []);

  if (movies.length === 0) return;

  return (
    <div className="mainWrapper">
      <MainBox movies={movies.results.drama} theme={MOVIE_TITLE[0]} />
      <MainBox movies={movies.results.america} theme={MOVIE_TITLE[1]} />
      <MainBox
        movies={movies.results.running_time_below_hundred}
        theme={MOVIE_TITLE[2]}
      />
    </div>
  );
};

export default Main;

const MOVIE_TITLE = [
  { id: 1, title: "드라마" },
  { id: 2, title: "미국" },
  { id: 3, title: "100분 순삭" },
];
```
- 영화목록의 테마는 '드라마', '미국', '100분 순삭'으로 영화를 나누었다.


<br />

<br />




## :: 성장 포인트 (해당 기능을 구현하며 고민했던 사항이나 새로 알게된 부분, 어려웠던 점 등을 작성합니다.)

> [6/21]

SCSS를 작성하면서 13인치 모니터에서는 영화 포스터가 5개만 나오게 설정했는데 큰 화면으로 옮겨서 확인하니 5개 반이 나타난다. 
[위의 문제 해결]
`width`를 %에서 px로 수정 또는 자식의 `width`를 `min-width`로 부여하기 
만약 `min-width`를 부모의 50%로 작성하면 그 이하로는 줄어들지 않기 때문에 부모에 맞춰 자식들이 끼어있는 것을 방지

`preBtn`과 `nextBtn` 위치를 `position: absolute`로 부여했는데 큰 화면으로 옮기면 엉뚱한 위치에 배치됨
[위의 문제 해결]
`position: relative`를 어디에 부여했는지 double check하기!

> [6/22]

슬라이드 구현에서 `prevBtn`이 생성되었다가 사라지지만 이미 원래의 위치로 돌아온 후에 한 번 더 클릭을 해야 버튼이 사라진다. `nextBtn`은 다음으로 넘어갈 슬라이드가 없어도 버튼이 사라지지 않는다. 모든 범위를 px로 주어서 그렇다.
현재는 이렇게 지정해도 `<FilmList>`컴포넌트가  10개로 정해져 있기 때문에 문제가 되지 않는데 추후 데이터가 추가 되거나 삭제 될 때의 경우도 생각하면 px을 기준으로 슬라이드를 이동하면 안될 것 같다는 느낌...
 
[위의 문제 해결]
멘토님께 여쭤보니 px로 하게되면 아주 복잡해지기 때문에 각각의 `<FilmList>`컴포넌트의 인덱스 값으로 배열을 사용하라고 알려주심. 

문제는 아직 해결하지 못했다.

>[6/23]

아직 슬라이드 구현을 제대로 하지 못했다. 오늘까지 해보자
[위의 문제 해결]
해당 사항 없음

>[6/24]

MockData를 불러오는 과정에서 `useState`를 사용했을 때 초기값을 빈 배열을 주고 `fetch`함수가 렌더링 되면서 그때 배열 안에 데이터가 담긴다. 이 부분을 간과하고 `{movies[0].country}`를 불러왔었다. 에러가 발생했다. 
"Cannot read properties of undefined." 
[위의 문제 해결]
원하는 데이터를 가져오기 위해 빈 배열이 아닐 떄 데이터를 불러오도록 조건문을 추가했다.
```js
<p className="filmTheme">{movies.length && movies[1].country}</p>
```
빈 배열을 표현하기 위해서는 `movies`의 길이 즉, `length`가 0일 떄는 `falsy`한 값이기 때문에 다음 명령은 실행되지 않는다. 빈 배열이 아닐 때는 무엇인가 담기기 때문에 `truthy`를 반환하여 다음 명령문을 실행한다.

>[6/27]

main페이지와 서버의 통신
```js
<Route path="/" element={<Main />} /> 
//내가 작업하는 메인페이지

<Route path="/detail/:id" element={<Detail />} />
//각 항목을 클릭하면 이동하는 상세페이지

<Link to={`/detail/${id}`} className="filmDetail">
//각 항목에 부여된 id값을 매개변수로 받아 해당 영화의 상세페이지로 이동
```
동기의 도움을 받아 작성하긴 했지만 어떤 로직으로 돌아가는지 정확하게 이해하지 못했다.
Query Parameter를 백에서 넘겨주고 프론트는 그것을 fetch함수에 작성한다.(질의문이기 때문에 조건에 부합하는 페이지 모두 불러온다.)
Path Parameter는 각각의 항목들에 부여된 고유값이 엔드포인트 다음에 작성된다. 대부분 id 값(조건이 아닌 id값에 해당하는 정보를 가져온다.)

>[6/28]

백엔드와의 소통, 협업....
서로의 언어가 다르다보니 서로의 로직을 설명할 때 이해하지 못한다. 정확히 csv, map함수가 무엇인지 모르기 때문이다. 이번 프로젝트로 가장 뼈저리게 느낀 것은 데이터 테이블을 짤 때 프론트는 백의 일이라고 생각하는 것이 아니라 나중에 데이터가 들어왔을 때 프런트가 고생하지 않으려면 무조건 같이 머리를 맞대고 같이 만들어 나가야 한다. 프로젝트 초반, 프런트는 레이아웃 짜기 바쁘고, 백은 데이터를 어떻게 구성할지 각자의 역할에 몰두한다. 하지만 현재 데이터에 대한 소통의 부재로 많은 시간과 노력이 의미없이 낭비되고 있다. 따라서 처음에 서로의 일이라고 무관심하는 것이 아니라 결국은 모두 연결되어 있기 때문에 효율적인 협업을 끝없이 진행해야 한다. 
