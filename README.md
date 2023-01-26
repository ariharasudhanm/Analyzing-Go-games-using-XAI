# xai_approaches
State visualization using XAI

<div id="top"></div>
<!--


<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->

<div align="center">
  
[![Contributors][contributors-shield]]()
[![Last-commit][last commit-shield]]()
[![license-url][license-shield]]()
[![LinkedIn][linkedin-shield]]()
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
  <h3 align="center">Image classification for Kaggle Competetion </h3>

  <p align="center">
    Classification of Kenyan foods with transfer learning methods using Pytorch
    <br />
    <a href="https://github.com/ariharasudhanm/Image_classification_Kaggle_Competition"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <!-- <a href="https://github.com/othneildrew/Best-README-Template">View Demo</a> -->
    ·
    <a href="https://github.com/ariharasudhanm/Image_classification_Kaggle_Competition/issues">Report Bug</a>
    ·
    <a href="https://github.com/ariharasudhanm/Image_classification_Kaggle_Competition/graphs/community">Request Feature</a>
  </p>
</div>


<!-- ABOUT THE PROJECT -->
## About The Project

- We have taken the state visualization of GO game played by AI trained alogorithms and Human played games.
The game is taken from three different sources AlphaGo archives, GoKifu, computer go datasets where each games are stored in SGF format.
Then we used this jku-vds-lab/projection-space-explorer under which notebook called alphago_notbook.ipynb used to prepare each and every states of the game.
The prepared datasets are consists of two different competetion type one is Human versus Human and Human versus AI algorithms each composed of several games played by AlphaGO and several professional GO players which can be found under data/Go. The dataset has totally 4132 rows and 365 columns. Rows are composed of each and every index of each game, and the state_type it belongs to whether it is start or intermediate or end, competitors (who are the players), competetion type and each and every places of the board.
Here we tried to analyze
How do professional players and AI start and end the games.
How does each and every state of the game changes?
Are there any similarities between professional players and AI moves,
Are there any specific strategies used by the AI or professional players.
We were expecting to see huge difference between AI and professional's moves since we know that AI is trained each and every day with new techniques, other expectations should be that AI should have some unique pattern such as highly defensive or highgly offensive against its players.


Project Overview:
* State visualization of games played.
* Data preparation (states).
* Visualization results.

<p align="center" width="75%">
       <img width="75%" src="https://user-images.githubusercontent.com/49080561/189544835-6bacf23c-78d2-4b55-8cd9-fcb0f942a572.png">
     </p>



<p align="right">(<a href="#top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Usage
* All the codes can be found under the `main.pynb` from data to preparation to training the model.
* Make sure to change the paths of all the files to your requirements where-ever needed if your'e training for a new model.
* Complete data used in this project is available in [OpenCV Pytorch Course - Classification](https://www.kaggle.com/competitions/opencv-pytorch-dl-course-classification/data).
* Some sample images used to train can be found under `Sample_data` directory.
* Trained model can be downloaded from [model.pth](https://drive.google.com/drive/folders/1MnlHoSVOOMgoyY1_6N8eOo2r2VeX6cg8?usp=sharing).



<!-- ROADMAP -->
## Roadmap

- [x] Data preparation.
- [x] Training and validation, Testing.
- [x] Hyperparameter Tuning.
- [x] Running docker container for inference.
- [x] Publishing the model as app.


See the [open issues](https://github.com/ariharasudhanm/Image_classification_Kaggle_Competition/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#top">back to top</a>)</p>


<!-- Results -->
## Results

Testing the trained model for few images from test set `tested_samples.png`.
<p align="center" width="55%">
       <img width="55%" src="https://user-images.githubusercontent.com/49080561/189545478-d5a5951d-20d2-4480-b54e-964a3842554b.png">
     </p>

<!-- ![Tested_samples](https://user-images.githubusercontent.com/49080561/189534349-c92d2bc3-88fa-4b8a-ab78-274f9c0a8833.png) -->


<!-- DOCKER CONTAINER -->
## Docker Container 

This section is composed of instructions to run a docker container for inferencing an image in the local machine(Linux).

1. You can pull the docker image to your local machine by using this command `docker pull ariharasudhan/food-classifier` in a command terminal, by default it will pull the latest image so no issues with image versions.
2. You can check the availability of this image in the local host by using `docker images ls -a` in a command terminal which should list down all the images including `img-classifier` which we are going to use to build a docker container.
3. Now you can run the command `docker run --name {name_of_your_container} --rm  -it -v {img_dir/path/in/localhost}:/usr/src/files/{new_dir}  img-classifier bash` which will create a new container and new volume called `new_dir` inside the container and mount the local directory which has images to the newly created container in the `new_dir` itself.
4. Now we should be inside that container in `/usr/src/files` this directory if you use `ls` command then you should be able to see the `new_dir` which you created earlier.
5. Using `python3 --image {new_dir/name_of_img.jpeg}` should list down the predictions with the top three probabilities.
7. Use `exit` command to exit the container since, we are using the `--rm` tag we will loose this container after exiting.
8. If you list down all the containers using `docker ps -a` or `docker container list ls` previously created container will not be there.



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

Project Link: [Image-classification-Kaggle-Competition](https://github.com/ariharasudhanm/Image_classification_Kaggle_Competition)

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
