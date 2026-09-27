<a id="readme-top"></a>

<div align="center">
  <a href="https://github.com/jerichd4c/java-practices-cohen/tree/main/java-stress-thread">
    <img src="https://raw.githubusercontent.com/jerichd4c/ReflexJDBC/main/java_logo.svg" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Java Stress Thread</h3>

  <p align="center">
    A minimalist Java tool for executing database stress tests over JDBC configurations.
  </p>
</div>

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#about-the-project">About The Project</a></li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

## About The Project

This is a ightweight demonstration repository that features a multithreaded stress testing class designed to evaluate database connection logic.

### Key Features:
* **Multithreading**: Employs Java Threads to simulate concurrent database accesses.
* **Minimalist Design**: Zero external dependencies (other than your JDBC driver).

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Built With

* [![Java][Java-shield]][Java-url]
* [![PostgreSQL][PostgreSQL-shield]][PostgreSQL-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Getting Started

To get a local copy up and running, follow these steps.

### Prerequisites

* Java JDK 11 or higher
* PostgreSQL Database

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/jerichd4c/java-practices-cohen.git
   ```
2. Navigate to the project directory
   ```sh
   cd java-practices-cohen/java-stress-thread
   ```
3. Download the [PostgreSQL JDBC Driver](https://jdbc.postgresql.org/download/).
4. **Mandatory Step**: Place the `.jar` file in your project root and **add it to your project's classpath** in your IDE:
    * **VS Code**: Go to the "Java Projects" view, find "Referenced Libraries", click the `+` icon, and select the `.jar` file in your project root.
    * **IntelliJ IDEA**: Go to `File -> Project Structure -> Libraries`, click `+`, select `Java`, and pick the `.jar` file in the project root.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Usage

```java
import pruebaestres.core.*;

// Run the static main method to begin the evaluation
PruebaDeEstres.main(new String[]{});
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## License

Distributed under the MIT License.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Acknowledgments
* [PostgreSQL JDBC Driver](https://jdbc.postgresql.org/download/)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
[Java-shield]: https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white
[Java-url]: https://www.java.com/
[PostgreSQL-shield]: https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white
[PostgreSQL-url]: https://www.postgresql.org/
