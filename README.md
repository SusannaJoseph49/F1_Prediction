<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="">
    <img src="Images/f1logo.jpg" alt="Logo" width="250" height="250">
  </a>
  <h3 align="center">Formula 1 Time Series Lap time Predictor</h3>
</p>
<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about">About</a>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#datasets">Datasets</a></li>
        <li><a href="#data-preprocessing">Data Preprocessing</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#authors">Authors</a></li>
    <li><a href="#acknowledgements">Acknowledgements</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About

We aim to predict qualifying lap times in Formula 1 using a driver–circuit specific deep learning model. By leveraging historical F1 race data and modeling each driver’s performance at each circuit, we developed a specialized forecasting system that achieves high accuracy with an average error of just 0.20% for seen data and 1.25% for unseen data.

[Full Project](https://github.com/SusannaJoseph49/F1_Prediction)


## Getting Started
Formula 1, despite being a proprietary and commercialized sport, has a surprisingly rich and open dataset ecosystem available to developers, analysts, and fans. Thanks to community-driven efforts and official data initiatives, you can access decades of detailed historical data on drivers, circuits, lap times, pit stops, qualifying results, and more.

### Datasets

The historical Formula 1 data was pulled from the [open source dataset avaliable on kaggle](https://www.kaggle.com/datasets/rohanrao/formula-1-world-championship-1950-2020).

The 2025 data for the ongoing season was taken from the official [F1 website](https://www.formula1.com/) for testing purposes. [Australia](https://www.formula1.com/en/results/2025/races/1254/australia/qualifying), [China](https://www.formula1.com/en/results/2025/races/1255/china/qualifying), [Japan](https://www.formula1.com/en/results/2025/races/1256/japan/qualifying), [Saudi Arabia](https://www.formula1.com/en/results/2025/races/1258/saudi-arabia/qualifying), [Miami](https://www.formula1.com/en/results/2025/races/1259/miami/qualifying), [Emilia-Romagna](https://www.formula1.com/en/results/2025/races/1260/emilia-romagna/qualifying) and [Monaco](https://www.formula1.com/en/results/2025/races/1261/monaco/qualifying) were taken into consideration. This [dataset](Data/2025_data/2025_qualifying_data.csv) can be expanded as the season progresses. 

### Data Preprocessing

Each Formula 1 circuit has unique characteristics (e.g. corners, elevation, surface, length), and drivers have track-specific strengths. By isolating data to one driver + circuit combination the model learns just one pattern: how that specific driver improves or regresses on that track over time. 
Another factor which influences the performances of various driver are the team they are with. The livery highly dictates the performance. So we include the team and temmate information also with each driver - circuit combination. 
<a href="">
    <img src="Images/ham.png" alt="ham">
  </a>




  ```sh
  conda env export > requirements.yml
  ```

The user will be able to recreate it using:

  ```sh
  conda env create -f requirements.yml
  ```

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/catiaspsilva/README-template.git
   ```
2. Setup (and activate) your environment
  ```sh
  conda env create -f requirements.yml
  ```

<!-- USAGE EXAMPLES -->
## Usage

Use this space to show useful examples of how a project can be used. For course projects, include which file to execute and the format of any input variables.

Additional screenshots, code examples and demos work well in this space. You may also link to more resources.

_For more examples, please refer to the [Documentation](https://example.com)_

<!-- ROADMAP -->
## Roadmap

See the [open issues](https://github.com/catiaspsilva/README-template/issues) for a list of proposed features (and known issues).

<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request


<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.


<!-- Authors -->
## Authors

Your Name - [@your_twitter](https://twitter.com/your_username) - email@example.com

Project Link: [https://github.com/your_username/repo_name](https://github.com/your_username/repo_name)


<!-- ACKNOWLEDGEMENTS -->
## Acknowledgements

You can acknowledge any individual, group, institution or service.
* [Catia Silva](https://faculty.eng.ufl.edu/catia-silva/)
* [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet)
* [Img Shields](https://shields.io)
* [Choose an Open Source License](https://choosealicense.com)
* [GitHub Pages](https://pages.github.com)
* [Animate.css](https://daneden.github.io/animate.css)
* [Loaders.css](https://connoratherton.com/loaders)
* [Slick Carousel](https://kenwheeler.github.io/slick)

## Thank you

<!-- If this is useful: [![Buy me a coffee](https://www.buymeacoffee.com/assets/img/guidelines/download-assets-sm-1.svg)](https://www.buymeacoffee.com/catiaspsilva) -->
