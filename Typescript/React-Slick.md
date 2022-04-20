# 🎞 React-Slick

> 리액트에서 Carousel을 쉽게 만들어주는 라이브러리
> Github = https://github.com/akiran/react-slick



## 설치 

```
npm install react-slick --save
yarn install react-slick


```

**After have to include CSS in project**

```
npm install slick-acrousel --save

import "~slick-carousel/slick/slick.css"; 
import "~slick-carousel/slick/slick-theme.css";
```



## 코드

```react
import React, { Component } from "react";
import Slider from "react-slick";
import "slick-carousel/slick/slick.css";
import "slick-carousel/slick/slick-theme.css";

const Slick = () => {
  const settings = {
    dots: true,
    fade: true,
    infinite: true,
    speed: 500,
    slidesToShow: 3,
    slidesToScroll: 1
  }
  return (
    <div>
      <h2>Fade</h2>
      <Slider {...settings}>
        <div>
          <img src="./logo192.png" style={{margin: 'auto'}}/>
        </div>
        <div>
          <img src="http://placekitten.com/g/400/200" style={{margin: 'auto'}}/>
        </div>
        <div>
          <img src="./logo192.png" style={{margin: 'auto'}}/>
        </div>
        <div>
          <img src="http://placekitten.com/g/400/200" style={{margin: 'auto'}}/>
        </div>
      </Slider>
    </div>
  );
}
export default Slick;
```



## 커스터마이징 settings

```react
  const settings = {
    dots: true,
    fade: true,
    infinite: true,
    speed: 500,
    slidesToShow: 3,
    slidesToScroll: 1
  }
```



- dots
  - Carousel 밑에 지정 콘텐츠로 이동할 수 있는 버튼
- infinite
  - 콘텐츠 끝까지 갔을 때 다음 콘텐츠로 처음 콘텐츠로 가져와 `반복`
- speed
  - 콘텐츠를 넘어갈 때 `속도`
  - 단위는 `ms`
- slidesToShow
  - 한 화면에 보이는 `콘텐츠 갯수`
- slidesToScroll
  - 한번에 넘어가는 `콘텐츠 수`
