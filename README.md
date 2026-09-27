<a id="readme-top"></a>

<br />
<div align="center">
  <img src="https://img.shields.io/badge/Java%20Practices-URU-blue?style=for-the-badge" alt="Java Practices" width="320" height="40">

<h3 align="center">Java Practices - Sebastian Cohen</h3>

  <p align="center">
    Repository for the Visual Programming course at URU. It gathers the final versions of the class exercises and projects, mostly Java programming practices around JDBC, connection pooling, and reflective sockets.
  </p>
</div>

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-repository">About The Repository</a>
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
    <li><a href="#repository-structure">Repository Structure</a></li>
    <li><a href="#main-projects">Main Projects</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
  </ol>
</details>

## About The Repository

This repository brings together the material covered in the **Visual Programming** course at URU. Despite the name, the coursework turned out to be mostly backend/systems Java practice rather than visual/GUI work, so this repository is named after what it actually contains: JDBC connection pooling, multithreaded stress testing, and reflective socket-based remote method execution.

Each project folder is self-contained and has its own README with setup instructions and implementation details.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Built With

* [![Java][Java-badge]][Java-url]
* [![PostgreSQL][PostgreSQL-badge]][PostgreSQL-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Getting Started

Each project has its own dependencies and run instructions — see its individual README linked in [Main Projects](#main-projects).

### Prerequisites

* Java JDK 11 or higher
* A PostgreSQL database (for the projects that connect to one)
* The [PostgreSQL JDBC Driver](https://jdbc.postgresql.org/download/), added manually to your IDE's classpath (none of these projects use a build tool like Maven/Gradle to manage it)

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/jerichd4c/java-practices.git
   ```
2. Open the folder for the project you want to run.
3. Follow that project's own README.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Repository Structure

These are the projects currently available in the repository:

* `ReflexJDBC/`: a database abstraction layer with connection pooling, externalized SQL queries, and multi-database configuration support.
* `java-connection-pool/`: a standalone, thread-safe JDBC connection pool with dynamic sizing.
* `java-stress-thread/`: a minimal multithreaded stress-testing tool for exercising database connection logic.
* `reflective-web-socket/`: a distributed system that invokes methods on remote objects over TCP sockets using Java reflection.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Main Projects

These are the projects developed during the course. Each one has its own internal documentation.

### [ReflexJDBC](ReflexJDBC/README.md)
A Java database abstraction layer: connection pooling, externalized SQL queries via property files, transaction handling, and support for switching between multiple configured databases.
* **Features**: connection pooling, query externalization, multi-DB configuration.
* **Documentation**: [Project README](ReflexJDBC/README.md)

### [Java Connection Pool](java-connection-pool/README.md)
A standalone, minimalist JDBC connection pool built independently of ReflexJDBC, focused purely on efficient connection reuse.
* **Features**: dynamic pool growth, thread-safe access, a built-in stress test suite.
* **Documentation**: [Project README](java-connection-pool/README.md)

### [Java Stress Thread](java-stress-thread/README.md)
A lightweight multithreaded tool for stress-testing database connection logic under concurrent load.
* **Features**: simulated concurrent database access via Java threads, zero external dependencies beyond the JDBC driver.
* **Documentation**: [Project README](java-stress-thread/README.md)

### [Reflective Web Socket](reflective-web-socket/README.md)
A distributed system where a client invokes methods on server-side business objects dynamically, using Java reflection over plain TCP sockets.
* **Features**: three concurrent socket servers (Calculator, Text Modifier, Converter), dynamic method dispatch via reflection.
* **Documentation**: [Project README](reflective-web-socket/README.md)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Roadmap

This roadmap summarizes the course progress and can keep growing as new units or assignments are added.

- [x] JDBC connection pooling and a reusable database abstraction layer (ReflexJDBC).
- [x] A standalone connection pool implementation.
- [x] Multithreaded stress testing of database connections.
- [x] Reflective remote method execution over TCP sockets.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

[Java-badge]: https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white
[Java-url]: https://www.java.com/
[PostgreSQL-badge]: https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white
[PostgreSQL-url]: https://www.postgresql.org/
