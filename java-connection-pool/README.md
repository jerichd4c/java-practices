<a id="readme-top"></a>

<div align="center">
  <a href="https://github.com/jerichd4c/java-practices/tree/main/java-connection-pool">
    <img src="https://raw.githubusercontent.com/jerichd4c/ReflexJDBC/main/java_logo.svg" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Java Connection Pool</h3>

  <p align="center">
    A high-performance, minimalist JDBC connection pool for Java applications.
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

This proyect is a lightweight, efficient JDBC connection pool designed for Java applications that require robust connection management with minimal overhead. It features dynamic pool growth, singleton access, and a built-in stress testing suite.

### Key Features:
* **Dynamic Sizing**: Automatically grows the pool based on demand up to a maximum limit.
* **Thread-Safe**: Uses synchronization and optimized collections for concurrent access.
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
   git clone https://github.com/jerichd4c/java-practices.git
   ```
2. Navigate to the project directory
   ```sh
   cd java-practices/java-connection-pool
   ```
3. Download the [PostgreSQL JDBC Driver](https://jdbc.postgresql.org/download/).
4. **Mandatory Step**: Place the `.jar` file in your project root and **add it to your project's classpath** in your IDE:
    * **VS Code**: Go to the "Java Projects" view, find "Referenced Libraries", click the `+` icon, and select the `.jar` file in your project root.
    * **IntelliJ IDEA**: Go to `File -> Project Structure -> Libraries`, click `+`, select `Java`, and pick the `.jar` file in the project root.
5. Configure your database settings in `src/main/resources/configSQL.properties`.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Usage

```java
import pooldeconexiones.core.*;

// Initialize the Pool through Manager
PoolManager manager = new PoolManager();
manager.crearPool();

// Get a connection
Connection conn = manager.getConnection();

// Use the connection...

// Return to pool
manager.returnConnectiontoPool(conn);
```

For a full stress test example, see `src/main/java/pooldeconexiones/demo/PruebaDeEstres.java`.

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
