# ๐ React-Slick

> ๋ฆฌ์กํธ์์ Carousel์ ์ฝ๊ฒ ๋ง๋ค์ด์ฃผ๋ ๋ผ์ด๋ธ๋ฌ๋ฆฌ
> Github = https://github.com/akiran/react-slick



## ์ค์น 

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



## ์ฝ๋

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



## ์ปค์คํฐ๋ง์ด์ง settings

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
  - Carousel ๋ฐ์ ์ง์  ์ฝํ์ธ ๋ก ์ด๋ํ  ์ ์๋ ๋ฒํผ
- infinite
  - ์ฝํ์ธ  ๋๊น์ง ๊ฐ์ ๋ ๋ค์ ์ฝํ์ธ ๋ก ์ฒ์ ์ฝํ์ธ ๋ก ๊ฐ์ ธ์ `๋ฐ๋ณต`
- speed
  - ์ฝํ์ธ ๋ฅผ ๋์ด๊ฐ ๋ `์๋`
  - ๋จ์๋ `ms`
- slidesToShow
  - ํ ํ๋ฉด์ ๋ณด์ด๋ `์ฝํ์ธ  ๊ฐฏ์`
- slidesToScroll
  - ํ๋ฒ์ ๋์ด๊ฐ๋ `์ฝํ์ธ  ์`
