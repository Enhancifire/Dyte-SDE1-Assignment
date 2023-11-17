<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a name="readme-top"></a>

<div align="center">

<h3 align="center">Log Searcher 10k</h3>

  <p align="center">
	Dyte SDE Assessment Project
    <br />
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

[![Log Searcher 10K][product-screenshot]](https://github.com/dyte-submissions/november-2023-hiring-Enhancifire)

Log Ingester and Query Tool built using Django for Dyte SDE Assessment. 

<p align="right">(<a href="#readme-top">back to top</a>)</p>



### Built With

* Python
* Django
* PostgreSQL
* SQLite3
* Docker

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

The project can be run using a local SQLite database, or using Docker. Both methods are described below.

### Prerequisites

- Python 3.10 or higher
- Docker (optional)

### Installation

#### Without Docker

1. Clone the repo
   ```sh
   git clone https://github.com/dyte-submissions/november-2023-hiring-Enhancifire.git
   ```
2. Create virtual environment
   ```sh
   python -m venv .env
   ```
3. Activate the environment
   ```sh
   source .env/bin/activate.fish # for fish shell
   ```

4. Install requirements
   ```sh
    pip install -r requirements.txt
   ```
  
5. Run migrations
   ```sh
    python manage.py migrate
    ```

6. Run the server
   ```sh
    python manage.py runserver 3000
   ```

#### With Docker

1. Clone the repo
   ```sh
   git clone https://github.com/dyte-submissions/november-2023-hiring-Enhancifire.git
   ```
2. Switch branch to docker
    ```sh
    git checkout docker
    ```
3. Start DB and build docker image
    ```sh
    docker compose up db -d
    ```

4. Build and Start the server
    ```sh
    docker compose up server --build
    ```
5. Run migrations
    ```sh
    docker compose exec server python manage.py migrate
    ```
6. Access the server at `localhost:3000`


<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage

Access the server at `localhost:3000`

Endpoints:
- '/': Home page
  Query interface is accessible here

- '/logs/': Ingest point for logs
  POST request to add individual logs to the database

- '/logsearch/': Search endpoint for logs
  Query interface accesses this endpoint to search for logs

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTACT -->
## Contact

Faiz Saiyad - +91 8177941560 - fsaiyad990@gmail.com

Project Link: [https://github.com/dyte-submissions/november-2023-hiring-Enhancifire](https://github.com/dyte-submissions/november-2023-hiring-Enhancifire)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/Enhancifire/repo_name.svg?style=for-the-badge
[contributors-url]: https://github.com/dyte-submissions/november-2023-hiring-Enhancifire/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/Enhancifire/repo_name.svg?style=for-the-badge
[forks-url]: https://github.com/dyte-submissions/november-2023-hiring-Enhancifire/network/members
[stars-shield]: https://img.shields.io/github/stars/Enhancifire/repo_name.svg?style=for-the-badge
[stars-url]: https://github.com/dyte-submissions/november-2023-hiring-Enhancifire/stargazers
[issues-shield]: https://img.shields.io/github/issues/Enhancifire/repo_name.svg?style=for-the-badge
[issues-url]: https://github.com/dyte-submissions/november-2023-hiring-Enhancifire/issues
[license-shield]: https://img.shields.io/github/license/Enhancifire/repo_name.svg?style=for-the-badge
[license-url]: https://github.com/dyte-submissions/november-2023-hiring-Enhancifire/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/faiz-saiyad
[product-screenshot]: images/screenshot.png
