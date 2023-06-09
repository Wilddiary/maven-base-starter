<h1 align="center" style="font-weight: bold; margin-top: 20px; margin-bottom: 20px;">maven-base-starter</h1>

<p align="center">

  <img alt="Github Build" src="https://img.shields.io/github/actions/workflow/status/Wilddiary/maven-base-starter/.github/workflows/maven-build.yml" />
  <img alt="Synk Vulnerabilities" src="https://img.shields.io/snyk/vulnerabilities/github/Wilddiary/maven-base-starter" />
  <img alt="GitHub Language Count" src="https://img.shields.io/github/languages/count/Wilddiary/maven-base-starter" />
  <img alt="GitHub Top Language" src="https://img.shields.io/github/languages/top/Wilddiary/maven-base-starter" />
  <img alt="GitHub Repo Size" src="https://img.shields.io/github/repo-size/Wilddiary/maven-base-starter" />
  <img alt="GitHub File Count" src="https://img.shields.io/github/directory-file-count/Wilddiary/maven-base-starter" />
  <img alt="GitHub Issues" src="https://img.shields.io/github/issues/Wilddiary/maven-base-starter" />
  <img alt="GitHub Closed Issues" src="https://img.shields.io/github/issues-closed/Wilddiary/maven-base-starter" />
  <img alt="GitHub Pull Requests" src="https://img.shields.io/github/issues-pr/Wilddiary/maven-base-starter" />
  <img alt="GitHub Closed Pull Requests" src="https://img.shields.io/github/issues-pr-closed/Wilddiary/maven-base-starter" />
  <img alt="GitHub Release" src="https://img.shields.io/github/v/release/Wilddiary/maven-base-starter?date_order_by=created_at&sort=date" />
  <img alt="GitHub Tag" src="https://img.shields.io/github/v/tag/Wilddiary/maven-base-starter" />
  <img alt="GitHub Contributors" src="https://img.shields.io/github/contributors/Wilddiary/maven-base-starter" />
  <img alt="GitHub Last Commit" src="https://img.shields.io/github/last-commit/Wilddiary/maven-base-starter" />
  <img alt="GitHub Commit Activity (Week)" src="https://img.shields.io/github/commit-activity/w/Wilddiary/maven-base-starter" />
  <img alt="GitHub Commit Activity (Month)" src="https://img.shields.io/github/commit-activity/m/Wilddiary/maven-base-starter" />
  <img alt="GitHub Commit Activity (Year)" src="https://img.shields.io/github/commit-activity/y/Wilddiary/maven-base-starter" />
  <img alt="Github License" src="https://img.shields.io/github/license/Wilddiary/maven-base-starter" />
  <img alt="Forks" src="https://img.shields.io/github/forks/Wilddiary/maven-base-starter" />
  <img alt="Followers" src="https://img.shields.io/github/followers/Wilddiary" />
  <img alt="Discussions" src="https://img.shields.io/github/discussions/Wilddiary/maven-base-starter" />

</p>

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

Includes GPG build plugin for signing the build artifacts. If you desire the artifacts should be signed then you need to configure GPG on your environment. Else, you can skip the signing process by setting the gpg.skip property to true either in your pom.xml or by passing it as a system property to maven.

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
