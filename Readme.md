# Big Data with Apache Spark
Welcome to the docs repository for Revature's 200413 Big Data/Spark cohort. Here you will find weekly topics, useful resources, and project requirements.

## Weekly Topics
Every week, we will focus on a particular technology or theme to add to our repertoire of competencies. These topics will feature heavily in assessments and QC meetings every week, and self-study and practical exploration will be necessary.
- [Week 1 - Java](week-1-java.md)
  - [Overview - Java](overview-java.md)
  - [Overview - Maven](overview-maven.md)
  - [Overview - Git](overview-git.md)
  - [Resources](resources-week-1.md)
- [Week 2 - SQL](week-2-linux-sql.md)
  - [Overview - PostgreSQL](overview-postgresql.md)
  - [Overview - JDBC](overview-jdbc.md)
  - [Overview - Linux](overview-linux.md)
  - [Resources](resources-week-2.md)
- [Week 3 - HTTP](week-3-http.md)
- [Week 4 - Big Data](week-4-big-data.md)
- [Week 5 - Apache Spark](week-5-apache-spark.md)
- [Week 6 - Spark SQL](week-6-spark-sql.md)
- [Week 7 - Spark Streaming](week-7-spark-streaming.md)

## Schedule & QC
[Google Doc](https://docs.google.com/document/d/1uVyBmeeKMbwQUCCiRurbpK1NBbpotbMsukZp2WLXtxk/edit?usp=sharing)

## Projects
This cohort will prioritize individual and group-based project work:
- [Project 0](project0.md): Begins Week 1, due **Wednesday Week 3**
- Project 1: Begins end of Week 3, due **Friday Week 5**
- Project 2: Begins Week 6, due **Friday Week 7**
- Project 3: Begins Week 8, due **Thursday Week 10**

Each project will require a list of features to be implemented, whether functional or operational, and finishing your MVP (minimum viable product) as early as possible before iterating new features upon the project is highly suggested. Plan ahead, and be sure to reach out to everyone whenever you require guidance (or offer your own to those in need).

## Developmemt Environment
To maximize resources and minimize troubleshooting, please perform a clean install or refresh of your operating system. Update your system, [Enable VT-x in BIOS](https://www.wikihow.tech/Enable-VT%E2%80%90x-in-BIOS) if possible, and uninstall all unnecessary programs. Your development environment should be set up for Java, Git, and Maven as soon as possible. In later weeks we will also require PostgreSQL, Docker, SSH, curl, and of course Apache Spark. Refer to this Readme or the links provided in each week's topic and resources document to keep updated on the latest tools and programs needed for project work. You will be responsible for maintaining your environment throughout the program.

## Tools
### Installers
- [Java in Visual Studio Code](https://code.visualstudio.com/docs/languages/java)

### Package Managers
- [Chocolatey for Windows](https://chocolatey.org)
- [Scoop for Windows](https://scoop.sh/)
- [Homebrew for MacOS/Linux](https://brew.sh/)

### Java SE 8 
* [AdoptOpenJDK](https://adoptopenjdk.net/)

### Command-line tools
* [Git](https://git-scm.com)
* [Apache Maven](https://maven.apache.org/)

### Editors
* [Visual Studio Code](https://code.visualstudio.com/)
- [Eclipse](https://www.eclipse.org/downloads/packages/)
- [IntelliJ IDEA](https://www.jetbrains.com/idea/)

## Installing Git, Java, Maven, and an IDE with Chocolatey (Windows only)
### Install [Chocolatey](https://chocolatey.org):
1. Open `Powershell` as an administrator.
1. Run:
    >Set-ExecutionPolicy AllSigned
1. Agree to all changes
1. Run:
    >Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))

### Install using Chocolatey
1. Open a new `Powershell` window as an administrator and run the following commands:
1. Install [Git for Windows](https://git-scm.com):
    >choco install git
1. Install [OpenJDK 8](https://adoptopenjdk.net/):
    >choco install adoptopenjdk8
1. Install [Apache Maven](https://maven.apache.org/):
    >choco install maven
1. Install an IDE of your choice:
   - Visual Studio Code:
        >choco install vscode
   - Eclipse:
        >choco install eclipse
   - IntelliJ IDEA community:
        >choco install intellijidea-community

### Summary
To confirm all tools are properly installed and configured, be sure the following commands return no errors:
```bash
git -v
java -version
javac -version
mvn -v
```

`java` and `javac` should only reference Java 1.8.

All above tools can be installed at once for convenience using the following command:
>choco install -y git adoptopenjdk8 maven vscode
