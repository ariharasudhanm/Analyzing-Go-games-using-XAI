
### How do Professional Go game players and AI plays the Go game?
### Any special strategies used by AlphaGo?

<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->

<div align="center">
  
[![Contributors][contributors-shield]](https://github.com/ariharasudhanm/Analyzing-Go-games-using-XAI/graphs/contributors)
[![Last-commit][last commit-shield]](https://github.com/ariharasudhanm/Analyzing-Go-games-using-XAI/graphs/commit-activity)
[![LinkedIn][linkedin-shield]](https://www.linkedin.com/in/ariharasudhan/)
<!-- [![license-url][license-shield]](https://github.com/ariharasudhanm/Image_classification_Kaggle_Competition/blob/main/LICENSE) -->
<!-- [![Forks][forks-shield]][forks-url] If needed add it later
[![Stargazers][stars-shield]][stars-url]  If needed add it later -->
 </p>
</div>




  
<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/ariharasudhanm/Image_classification_Kaggle_Competition">
    <!-- <img src="images/logo.png" alt="Logo" width="80" height="80"> -->
  </a>
  <h3 align="center">State visualization of Go game</h3>

  <p align="center">
    Comparing the Go games played between professionals and AI which is trained to play Go game.
    <br />
    <a href="https://github.com/ariharasudhanm/Analyzing-Go-games-using-XAI"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <!-- <a href="https://github.com/othneildrew/Best-README-Template">View Demo</a> -->
    ·
    <a href="https://github.com/ariharasudhanm/Analyzing-Go-games-using-XAI/issues">Report Bug</a>
    ·
    <a href="https://github.com/ariharasudhanm/Analyzing-Go-games-using-XAI/graphs/community">Request Feature</a>
  </p>
</div>


<!-- ABOUT THE PROJECT -->
## About The Project

- We tried to analyze the go games played between pioneers of go game AI which has been trained to play the go game using state visualization of GO game.
- The games are taken from three different sources [AlphaGo archives](https://homepages.cwi.nl/~aeb/go/games/games/AlphaGo/index.html), [GoKifu](http://gokifu.com/index.php?a=1&y=2020&m=11), [computer go datasets](https://github.com/yenw/computer-go-dataset) where each games are stored in SGF format.
- Then we used this [jku space explorer](https://github.com/jku-vds-lab/projection-space-explorer/tree/master/notebooks) under which notebook called `alphago_notbook.ipynb` used to prepare each and every states of the game.
- The prepared datasets are consists of two different competetion type one is Human versus Human and Human versus AI algorithms each composed of several games played by AlphaGO and several professional GO players which can be found under `data/Go`. The dataset has totally 4132 rows and 365 columns. Rows are composed of each and every index of each game, and the state_type it belongs to whether it is start or intermediate or end, competitors (who are the players), competetion type and finally what is there in each and every places of the board.
## Here we tried to analyze
>- How do professional players and AI start and end the games.
>- How does each and every state of the game changes?
>- Are there any similarities between professional players and AI moves?
>- Are there any specific strategies used by the AI or professional players.

Project Overview:
* State visualization of games played.
* Data preparation (states).
* Visualization results.

<p align="center" width="65%">
       <img width="65%" src="https://user-images.githubusercontent.com/49080561/215096119-c31cc655-43ba-4948-ab45-a8466cbfdebf.png">
     </p>

Here red circle shows ending pattern. 

We tried several projections such as PCA and TSNE. Both shown different patterns which can be observerd below.
<p align="center" width="65">
       <img width="65%" src="https://user-images.githubusercontent.com/49080561/215096607-deab9d10-cbab-4404-a85e-9482e679ad0e.png">
     </p>
Here we observed that humans playing strategies tend to differ a lot when compared to AI as we could clearly see that both regimes are well separated in the above plot.
<p align="right">(<a href="#top">back to top</a>)</p>

More patterns such as starting and ending patterns are well decribed in the `main.html` file which we highly reccomend to go through for completeness since it involves necessary explanations along with graphical parts.

<!-- GETTING STARTED -->
## Usage



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Your Name - [@AriharasudhanM](https://twitter.com/your_username) - ariharasudhan.muthusami@gmail.com

Project Link: [State Visualization using XAI](https://github.com/ariharasudhanm/Analyzing-Go-games-using-XAI)

<p align="right">(<a href="#top">back to top</a>)</p>




<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/ariharasudhanm/Image-classification-using-transfer-learning?color=Green&logoColor=Red&style=for-the-badge
[contributors-url]: https://github.com/ariharasudhanm/Image_classification_Kaggle_Competition/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/ariharasudhanm/Image_classification_Kaggle_Competition/blob/main/LICENSE
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
[product-screenshot]: images/screenshot.png

[Last-commit]: https://github.com/ariharasudhanm/Image_classification_Kaggle_Competition/graphs/commit-activity
[last commit-shield]: https://img.shields.io/github/last-commit/ariharasudhanm/Image_classification_Kaggle_Competition?style=for-the-badge
[matplotlib-shield]: https://img.shields.io/badge/Matplotlib-v3-Green
