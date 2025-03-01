[![Englsh][language-en-shield]](README.md) 
[![Korean][language-kr-shield]](README.kr.md)

![image](https://user-images.githubusercontent.com/1613812/125195363-365a7d00-e290-11eb-92b5-6cfd5266962e.png)

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![Build Status][build-status-shield]][build-status-url]
[![Quality Gate Status][quality-gate-status-shield]][quality-gate-status-url]
[![Coverage][coverage-shield]][coverage-url]

<!-- ABOUT THE PROJECT -->
# eGovFrame Runtime

eGovernment Standard Framework - Runtime Environment

## Description

Common modules necessary for the execution of business logic programs in eGovernment project. Application programming environment to facilitate the standardized development of screens, server programs and data.

<!-- GETTING STARTED -->
## Getting Started

eGovFrame Runtime uses the Maven framework. 

### Prerequisites

* Maven, version 3+
* Java JDK 1.7+

### How to build

#### Building it

This is a Maven project, and to build it use the following command:

```
$ mvn clean install
```

Optionally you can specify -Dmaven.test.skip=true to skip the tests (even though you shouldn't as you know)

The build result will be a eGovFrame Runtime package located in ```target```.

#### Packaging / Distributing it

Packages can be built by using the following command:

```
$ mvn clean package
```

The packaged results will be in the `target/` 

#### Running the tests

__Unit tests__

This will run all unit tests in the project (and sub-modules). 

```
$ mvn test
```

<!-- USAGE EXAMPLES -->
### Usage

eGovFrame Runtime can be downloaded using maven through the following settings in pom.xml file.

#### Using dependency definitions. 

After adding above, add the following dependency definitions. 
(Only the required ones.)

``` xml

<properties>
    <spring.maven.artifact.version>5.2.5.RELEASE</spring.maven.artifact.version>
    <org.egovframe.rte.version>4.0.0</org.egovframe.rte.version>
</properties>

...

<dependency>
    <groupId>egovframework.rte</groupId>
    <artifactId>egovframework.rte.fdl.cmmn</artifactId>
    <version>${egovframework.rte.version}</version>
</dependency>

<dependency>
    <groupId>egovframework.rte</groupId>
    <artifactId>egovframework.rte.ptl.mvc</artifactId>
    <version>${egovframework.rte.version}</version>
</dependency>

<dependency>
    <groupId>egovframework.rte</groupId>
    <artifactId>egovframework.rte.psl.dataaccess</artifactId>
    <version>${egovframework.rte.version}</version>
</dependency>

<dependency>
    <groupId>egovframework.rte</groupId>
    <artifactId>egovframework.rte.fdl.logging</artifactId>
    <version>${egovframework.rte.version}</version>
</dependency>

<!-- OPTIONAL -->
<dependency>
    <groupId>egovframework.rte</groupId>
    <artifactId>egovframework.rte.fdl.idgnr</artifactId>
    <version>${egovframework.rte.version}</version>
</dependency>

<!-- OPTIONAL -->
<dependency>
    <groupId>egovframework.rte</groupId>
    <artifactId>egovframework.rte.fdl.property</artifactId>
    <version>${egovframework.rte.version}</version>
</dependency>

...

```

## Version History

* 4.0.0 beta
    * Various bug fixes and optimizations
    * See [commit change]() or See [release history]()
* 4.0.0 alpha
    * Initial Release

<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b eGovFramework/egovframe-runtime`)
3. Commit your Changes (`git commit -m 'Add some egovframe-runtime'`)
4. Push to the Branch (`git push origin eGovFramework/egovframe-runtime`)
5. Open a Pull Request

## Asking for help

Please go to https://www.egovframe.go.kr/home/sub.do?menuNo=69 to ask questions and get help.

<!-- LICENSE -->
## License

The eGovFrame Framework is released under version 2.0 of the [Apache License](https://www.apache.org/licenses/LICENSE-2.0).

## Contact

Contributors names and contact info

ex. Project Link: [https://github.com/eGovFramework/egovframe-runtime](https://github.com/eGovFramework/egovframe-runtime)

<!-- MARKDOWN LINKS & IMAGES -->
[language-kr-shield]: https://img.shields.io/badge/language-Korean-blue.svg?style=flat-square
[language-en-shield]: https://img.shields.io/badge/language-English-red.svg?style=flat-square

[contributors-shield]: https://img.shields.io/github/contributors/eGovFramework/egovframe-runtime.svg?style=flat-square
[contributors-url]: https://github.com/eGovFramework/egovframe-runtime/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/eGovFramework/egovframe-runtime.svg?style=flat-square
[forks-url]: https://github.com/eGovFramework/egovframe-runtime/network/members
[stars-shield]: https://img.shields.io/github/stars/eGovFramework/egovframe-runtime.svg?style=flat-square
[stars-url]: https://github.com/eGovFramework/egovframe-runtime/stargazers
[issues-shield]: https://img.shields.io/github/issues/eGovFramework/egovframe-runtime.svg?style=flat-square
[issues-url]: https://github.com/eGovFramework/egovframe-runtime/issues
[license-shield]: https://img.shields.io/github/license/eGovFramework/egovframe-runtime.svg?style=flat-square
[license-url]: https://github.com/eGovFramework/egovframe-runtime/blob/master/LICENSE.txt

[build-status-shield]: https://shields.io/travis/openlenalab/egovframe-runtime?style=flat-square
[build-status-url]: https://app.travis-ci.com/openlenalab/egovframe-runtime
[quality-gate-status-shield]: https://sonarcloud.io/api/project_badges/measure?project=openlenalab_egovframe-runtime&metric=alert_status
[quality-gate-status-url]: https://sonarcloud.io/dashboard?id=openlenalab_egovframe-runtime
[coverage-shield]: https://sonarcloud.io/api/project_badges/measure?project=openlenalab_egovframe-runtime&metric=coverage
[coverage-url]: https://sonarcloud.io/dashboard?id=openlenalab_egovframe-runtime

