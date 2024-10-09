ISCTE-ScheduleManager
=====================

This project, was developed as part of a group assignment during my bachelor's degree at ISCTE. The main focus was to learn how to work with sprints, Git, and collaborative software development. It is a schedule management platform for ISCTE students, designed to manage academic timetables. The project was developed using JavaFX for the graphical interface and includes integration with other tools such as SonarCloud and GitHub Actions for continuous integration.

You can find the original repository, which includes the full commit history and team contributions, at this link:\
[Original Repository](https://github.com/AlfDozen/ES-2023-Sem2-Terca-Feira-LEIPL-GrupoA).

* * * * *

Project Overview (Translated from Portuguese)
---------------------------------------------

### Version: GestaodeHorarios-1.0

**Group Identification (Moodle):** Terça-Feira-LEIPL-GrupoA\
**Repository:** [ES-2023-Sem2-Terca-Feira-LEIPL-GrupoA](https://github.com/AlfDozen/ES-2023-Sem2-Terca-Feira-LEIPL-GrupoA)\
**SonarCloud:** [SonarCloud Project Overview](https://sonarcloud.io/project/overview?id=AlfDozen_ES-2023-Sem2-Terca-Feira-LEIPL-GrupoA)

### Group Members:

-   **Pedro Almeida** (Nº: 97960, GitHub: pmaaa2-iscte, Email: pmaaa2@iscte-iul.pt)
-   **Diogo Cardoso** (Nº: 98816, GitHub: diogocardoso777, Email: daoco@iscte-iul.pt)
-   **Alexander Ferreira** (Nº: 94481, GitHub: afarl-iscteiul, Email: afarl@iscte-iul.pt)
-   **Cláudia Ferreira** (Nº: 98184, GitHub: carfa2-iscte, Email: alexandra_rocha@iscte-iul.pt)
-   **Salvador Silva** (Nº: 98777, GitHub: salvadoriscte, Email: smvsa3@iscte-iul.pt)
-   **Vitor Silva** (Nº: 99149, GitHub: vitorhugo-iscteiul, Email: vhcsa@iscte-iul.pt)

* * * * *

Project Details
---------------

### Sprint 1:

-   **Errors Identified:** No errors were found.
-   **Unimplemented or Incomplete Features:**
    1.  From the backlog, some features are pending implementation (e.g., generating timetables based on data from Fénix, creating timetables by selecting subjects from a previously loaded schedule, visualizing overlapping classes, and visualizing overcrowded classes).
    2.  The graphical interface is incomplete but meets the goals set for Sprint 1.

### Sprint 2:

-   **Errors Identified:** No errors were found.
-   **Unimplemented or Incomplete Features:** None to report.

* * * * *

Code Quality
------------

### Code Smells Identified by SonarCloud:

-   **Critical Code Smells:** Seven critical issues related to static attributes used in non-static methods. These were found in the GUI classes and are considered to have no impact on the application.
-   **Major Code Smells:** Four major issues related to exceptions being caught and ignored (empty catch blocks) and suggestions for using a different import to improve error messages when deleting files.
-   **Minor Code Smells:** Four minor issues related to the use of static attributes and not implementing an `equals()` function when applying the `Comparable` interface.

SonarCloud also identified three minor bugs concerning how the code handles boolean returns when creating and deleting temporary files. According to our analysis, the code works as intended, and no changes are necessary.

* * * * *

JUnit Code Coverage:
--------------------

-   **Overall Coverage:** 64% according to cyclomatic complexity metrics, including all classes under `src/main/java`, including the GUI classes. The non-GUI classes have more than 90% coverage.

* * * * *

Continuous Integration:
-----------------------

We set up a workflow in GitHub Actions to automatically run build, JUnit tests, Javadoc validation, and SonarCloud integration upon each commit or pull request to the `main` branch.

* * * * *

Libraries Used:
---------------

-   **JavaFX**: <https://openjfx.io/>
-   **CalendarFX**: <https://github.com/dlsc-software-consulting-gmbh/CalendarFX>
-   **CSV and JSON Parsing**:
    -   [Jackson Core](https://mvnrepository.com/artifact/com.fasterxml.jackson.core/jackson-core)
    -   [Jackson Databind](https://mvnrepository.com/artifact/com.fasterxml.jackson.core/jackson-databind)
    -   [Jackson CSV](https://mvnrepository.com/artifact/com.fasterxml.jackson.dataformat/jackson-dataformat-csv)
