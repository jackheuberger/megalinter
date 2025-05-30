---
title: JAVA linters in MegaLinter
description: checkstyle, pmd are available to analyze JAVA files in MegaLinter
---
<!-- markdownlint-disable MD003 MD020 MD033 MD041 -->
<!-- @generated by .automation/build.py, please don't update manually -->
<!-- Instead, update descriptor file at https://github.com/oxsecurity/megalinter/tree/main/megalinter/descriptors/java.yml -->
# JAVA

## Linters

| Linter                                                                           | Additional                                                                                                                                                                                |
|----------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**checkstyle**](java_checkstyle.md)<br/>[_JAVA_CHECKSTYLE_](java_checkstyle.md) | [![GitHub stars](https://img.shields.io/github/stars/checkstyle/checkstyle?cacheSeconds=3600)](https://github.com/checkstyle/checkstyle) ![sarif](https://shields.io/badge/-SARIF-orange) |
| [**pmd**](java_pmd.md)<br/>[_JAVA_PMD_](java_pmd.md)                             | [![GitHub stars](https://img.shields.io/github/stars/pmd/pmd?cacheSeconds=3600)](https://github.com/pmd/pmd) ![sarif](https://shields.io/badge/-SARIF-orange)                             |

## Linted files

- File extensions:
  - `.java`

## Configuration in MegaLinter

| Variable                  | Description                                     | Default value |
|---------------------------|-------------------------------------------------|---------------|
| JAVA_PRE_COMMANDS         | List of bash commands to run before the linters | None          |
| JAVA_POST_COMMANDS        | List of bash commands to run after the linters  | None          |
| JAVA_FILTER_REGEX_INCLUDE | Custom regex including filter                   |               |
| JAVA_FILTER_REGEX_EXCLUDE | Custom regex excluding filter                   |               |


## Behind the scenes

### Installation

- Dockerfile commands :
```dockerfile
ENV JAVA_HOME=/usr/lib/jvm/java-21-openjdk
ENV PATH="$JAVA_HOME/bin:${PATH}"
```

- APK packages (Linux):
  - [openjdk21](https://pkgs.alpinelinux.org/packages?branch=v3.21&arch=x86_64&name=openjdk21)
