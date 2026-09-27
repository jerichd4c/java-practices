<a id="readme-top"></a>

<!-- PROJECT LOGO -->
<div align="center">
  <a href="https://github.com/jerichd4c/java-practices-cohen/tree/main/reflective-web-socket">
    <img src="https://raw.githubusercontent.com/jerichd4c/ReflexJDBC/main/java_logo.svg" alt="Logo" width="80" height="80">
  </a>
</div>


<div align="center">
  <h3 align="center">Reflective Socket Project</h3>

  <p align="center">
    A Java application that uses reflection and sockets to invoke methods on remote objects dynamically.
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
    <li><a href="#license">License</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About The Project

This project demonstrates a distributed system where a client can invoke methods on server-side objects using Java Reflection. The server hosts various business objects, and the client communicates over TCP sockets to execute logic remotely.

### Built With

* [![Java][Java-shield]][Java-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->
## Getting Started

To get a local copy up and running, follow these steps.

### Prerequisites

* Java Development Kit (JDK) 8 or higher.

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/jerichd4c/java-practices-cohen.git
   ```
2. Navigate to the project directory
   ```sh
   cd java-practices-cohen/reflective-web-socket
   ```
3. Compile the project (if using an IDE like IntelliJ, it will handle this automatically).
4. Run the `BusinessApp` class located in `src/main/java/reflectivesocket/BusinessApp.java`.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- USAGE EXAMPLES -->
## Usage

When you run `BusinessApp`, you will see a menu to interact with different remote services:

1. **Calculator**: Perform arithmetic operations.
2. **Text Modifier**: Manipulate strings.
3. **Converter**: Convert data formats.

The application starts three socket servers on ports 5000, 5001, and 5002 to handle these requests.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- LICENSE -->
## License

Distributed under the MIT License.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
[Java-shield]: https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white
[Java-url]: https://www.oracle.com/java/
