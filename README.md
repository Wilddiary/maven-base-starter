# maven-base-starter [![Release](https://github.com/Wilddiary/maven-base-starter/actions/workflows/maven-release.yml/badge.svg)](https://github.com/Wilddiary/maven-base-starter/actions/workflows/maven-release.yml)
Maven starter project with pre-configured build plugins. Provides basic dependencies and standard build experience.
Enforces the following quality gates.

1. Standard code style checks
2. Checkstyle based static code analysis
3. Dependency vulnerability scans
4. Enforces standard sorting of pom elements
5. Collects and reports code coverage stats
6. Readable junit execution reports.
7. Enforces JDK and maven versions.
8. On-demand dependency upgrade reports

### Usage ###
Just use it as a parent pom by inheriting it in your project pom. Inherited projects will have the standard build
experience with all quality gates defined by this project.
```xml
  <parent>
    <groupId>com.wilddiary</groupId>
    <artifactId>maven-base-starter</artifactId>
    <version>{version}</version>
    <relativePath />
  </parent>
```
