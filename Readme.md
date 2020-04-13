# Big Data with Apache Spark
Welcome to the docs repository for Revature's 200413 Big Data/Spark cohort. Here you will find weekly topics, useful resources, and project requirements.

## Weekly Topics
Every week, we will focus on a particular technology or theme to add to our repertoire of competencies. These topics will feature heavily in assessments and QC meetings every week, and self-study and practical exploration will be necessary.
- [Week 1 - Java](Week%201%20-%20Java.md)
  - [Overview - Java](Overview%20-%20Java.md)
  - [Overview - Maven](Overview%20-%20Maven.md)
  - [Overview - Git](Overview%20-%20Git.md)
- [Week 2 - SQL](Week%202%20-%20SQL.md)
- [Week 3 - HTTP](Week%203%20-%20HTTP.md)
- [Week 4 - Big Data](Week%204%20-%20Big%20Data.md)
- [Week 5 - Apache Spark](Week%205%20-%20Apache%20Spark.md)
- [Week 6 - Spark SQL](Week%206%20-%20Spark%20SQL.md)
- [Week 7 - Spark Streaming](Week%207%20-%20Spark%20Streaming.md)

## Projects
This cohort will prioritize individual and group-based project work:
- [Project 0](Project%200.md): Begins Week 1, due **Wednesday Week 3**
- Project 1: Begins end of Week 3, due **Friday Week 5**
- Project 2: Begins Week 6, due **Friday Week 7**
- Project 3: Begins Week 8, due **Thursday Week 10**

Each project will require a list of features to be implemented, whether functional or operational, and finishing your MVP (minimum viable product) as early as possible before iterating new features upon the project is highly suggested. Plan ahead, and be sure to reach out to everyone whenever you require guidance (or offer your own to those in need).

## Quality Control
The goal of this cohort is to gain professional software and data engineering skills and succeed on client project work in the future. To that end, we will conduct regular assessments, meetings, and 1:1 sessions and hold this cohort to a high standard. Associates should be expected to know and understand industry terminology, express themselves clearly and professionaly, and engage with their mentor and each other in a friendly and productive manner.

- Quizzes: Will be held every Monday on RevaturePro
- 1:1 sessions: Will be held every Monday to discuss personal progress and interpersonal skills
- QC meetings: Will be held every Monday or Tuesday to discuss topics from the week prior

## Developmemt Environment
To maximize resources and minimize troubleshooting, please perform a clean install or refresh of your operating system. Update your system, [Enable VT-x in BIOS](https://www.wikihow.tech/Enable-VT%E2%80%90x-in-BIOS) if possible, and uninstall all unnecessary programs. Your development environment should be set up for Java, Git, and Maven as soon as possible. In later weeks we will also require PostgreSQL, Docker, SSH, curl, and of course Apache Spark. Refer to this Readme or the links provided in each week's topic and resources document to keep updated on the latest tools and programs needed for project work. You will be responsible for maintaining your environment throughout the program.

## Tools
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
1) Install [Chocolatey](https://chocolatey.org)
     1) Open `Powershell` as an administrator.
     2) Run:
         >Set-ExecutionPolicy AllSigned
     3) Agree to all changes
     4) Run:
         >Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
2) Open a new `Powershell` window as an administrator and run the following commands:
3) Install [Git for Windows](https://git-scm.com):
    >choco install git
4) Install [OpenJDK 8](https://adoptopenjdk.net/):
    >choco install adoptopenjdk8
5) Install [Apache Maven](https://maven.apache.org/):
    >choco install maven
6) Install an IDE of your choice:
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
