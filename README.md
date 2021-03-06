<h1 align="center">TEMPLATE CLIENT ๐</h1>
<p>
  <img alt="Version" src="https://img.shields.io/badge/version-0.1.0-blue.svg?cacheSeconds=2592000" />
</p>

> ์ด๊ฒ์ ํํ๋ฆฟ ํด๋ผ์ด์ธํธ์๋๋ค

## Author

๐ค **Anderson**

- Website: https://chltjdrhd777.github.io/
- Github: [@chltjdrhd777@naver.com](https://github.com/chltjdrhd777@naver.com)
- Give a โญ๏ธ if this project helped you!

---

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]
<br/>
(_์ด๋ฌ๋ฉด ์ข๊ฒ ๋ค_)

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <h3 align="center">์ฌ์ฉ๋(ํน์ ์ฌ์ฉํ ) ์คํ๋ฆฌ์คํธ</h3>

- [ReduxToolkit](https://redux-toolkit.js.org/)
- [React.js](https://reactjs.org/)
- [Typescript](https://www.typescriptlang.org/)
- [EmotionCSS](https://emotion.sh/docs/introduction)
- [Bootstrap](https://getbootstrap.com)

---

# design structure

<div align="left">
<br/>

0. ์คํ์ผ์ ์คํ์ผ๋ก, ๊ธฐ๋ฅ์ ๊ธฐ๋ฅ์ผ๋ก ์ปดํฌ๋ํธ๋ฅผ ๊ตฌ๋ถํ์ฌ ๊ด์ฌ์ฌ๋ฅผ ๋ฐ๋ก๋๋ค

1. styled ํด๋์ index์๋ ์น ์ ์ฒด์์ ๊ณต์ฉ์ผ๋ก ์ฌ์ฉ๋  styled component๋ฅผ ์ ๋ฆฌํ๊ณ 

2. ๋์์ธ์ ์ธ ๋ณ๊ฒฝ์ ๊ทธ ๋ด๋ถ์์ class๋ฅผ ํตํด ์ ์ํจ์ ๋ฐ๋ผ ํ์์ ๋ฐ๋ผ bootstrap์ฒ๋ผ ํด๋์ค์ ๋ณ๊ฒฝ๋ง์ผ๋ก ๋์์ธ์ด ์ ๋์ ์ผ๋ก ๋ณ๊ฒฝ๋๊ฒ ํ๋ค

3. styled ํด๋ ์์ ๋ค์ด๋ฐ์ด ๋ ํ์ผ๋ค์ ๊ฐ route๋ฅผ ๋ปํ๋ฉฐ, ํด๋น ๋ด๋ถ์๋ index์ ๋ฒ ์ด์ค ์ปดํฌ๋ํธ๋ฅผ ๋ฌผ๋ ค๋ฐ์ ํด๋น ํ์ด์ง์์ ์ด๋ค ์ปดํฌ๋ํธ๊ฐ ์ฌ์ฉ๋๋์ง๋ฅผ ๊ด๋ฆฌํ๋ค.

4. ๋ํ media query๋ฅผ ๋ด๋ถ์ ๋ ์ผ๋ก์, ์ฌ์ฉ๋ ์ปดํฌ๋ํธ๋ค์ด ๋ฏธ๋์ด์ฟผ๋ฆฌ๋ฅผ ํตํด ์กฐ์ ๋๋๋ก ๋ง๋ ๋ค.

5. ๊ธฐ๋ฅ์ ์ธ ๋ถ๋ฆฌ๋ styled ์ธ๋ถ์ ๋ฐ๋ก ์ ์ํจ์ผ๋ก์, ๊ธฐ๋ฅ์  ์ฌํ์ฉ์ ๊ฟฐํ๋ค

</div>

---

# styled refactor principle

<<์คํ์ผ๋ง์ ์ํ styled ์ปดํฌ๋ํธ์ ๋ถ๋ฆฌ ๊ธฐ์ค์>>

<div align="left">
<br/>

1. styledํด๋ ๋ด์, ํ์ด์ง์ ์ด๋ฆ์ ๊ฐ์ง ํ์ผ์ ํ์ฑํ๊ณ , ๊ทธ ์์ ์ฐจ๋ก๋๋ก ์ ์ฅํ๋ค.(ex, Home.styled.ts). <br/>styled ์ปดํฌ๋ํธ๋ฅผ ๋๋๋ ๊ธฐ์ค์ ํฐ ๊ตฌํ๋ณ๋ก ๋๋๋ค _**(ex/ Main => Container => Nav => NavHeading, NavLists)**_

2. (optional) ๋ง์ฝ ํน์  ์ปดํฌ๋ํธ์ ํํ๊ฐ ๊ณ์ ๋ฐ๋ณต์ ์ผ๋ก ์ฌ์ฌ์ฉ๋๋ค๋ฉด, ํด๋น ํ์ด์ง๋ก ๋ช๋ชํ ํด๋ ๋ด์ component ํํ๋ก ๋ชจ์๋๋ค._**(ex, components/Home)**_<br/> ์ด๋ ํด๋น ์ปดํฌ๋ํธ๋ค์ ๋์ค์ mediaQuery๋ก์ styled.ts ํ์ผ์์ ์ ๊ทผ์ด ๊ฐ๋ฅํ๋๋ก ํด๋์ค๋ฅผ ๋ถ์ธ๋ค.

<br/>
์ฆ, ์ชผ๊ฐค๋๊น์ง ์ชผ๊ฐ์ ์ปดํฌ๋ํธ๋ก ๋ชฐ์์ฃผ๊ณ ๋์
<br/>
=> ํด๋์ค๋ก ๊ณตํต์ ์ผ๋ก ์ปจํธ๋กคํด์ผ๋  ๊ฒ ๊ฐ์ผ๋ฉด ์ชผ๊ฐ์ง ์๊ณ  ํด๋์ค๋ก ๋ถ์ฌ์ ์ฒ๋ฆฌ.
<br/>
=> ๊ณต์ฉ ์ปดํฌ๋ํธ์ฌ๋ ๋์ผํ๊ฒ ํด๋์ค๋ฅผ ๋ถ์ฌ์ ์ฒ๋ฆฌํ๋ค. ์ด๋ ๋์ค์ ๋ฏธ๋์ด ์ฟผ๋ฆฌ๋ ํต์ผ์ฑ์ ์ ์งํ๊ธฐ ์ํด์์ด๋ค.
</div>
<br/><br/>

> ํ ์์ญ์์๋ง ๊ณ์ ๋ฐ๋ณต๋๊ณ  ๋ค๋ฅธ ์์ญ์์ ์ฐ์ด์ง ์์ ๊ฒ ๊ฐ๋ค๋ฉด ๊ทธ๋ฅ ํด๋น ๋ด๋ถ์์ ํด๋์ค๋ช์ ์ง์ ํ์ฌ ์ฝ๋ฉํด๋ ๊ด์ฐฎ๋ค<br/>(routes/Home/sections/Hotels ์ ๊ทธ๋ฆฌ๋ ์์ญ ์ฐธ์กฐ)

---

## Contact

My Email - [@google](chltjdrhd777@gmail.com) - chltjdrhd777@gmail.com

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->

- [Choose an Open Source License](https://choosealicense.com)
- [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet)
- [Malven's Flexbox Cheatsheet](https://flexbox.malven.co/)
- [Malven's Grid Cheatsheet](https://grid.malven.co/)
- [Img Shields](https://shields.io)
- [GitHub Pages](https://pages.github.com)
- [Font Awesome](https://fontawesome.com)
- [React Icons](https://react-icons.github.io/react-icons/search)

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
