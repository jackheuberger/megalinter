<!-- markdownlint-disable MD033 MD041 -->
<!-- @generated by .automation/build.py, please do not update manually -->
# git_diff

Git diff checks for git conflicts markers in files

## git_diff documentation

- Version in MegaLinter: **2.30.2**
- Visit [Official Web Site](https://git-scm.com){target=_blank}

[![git - GitHub](https://gh-card.dev/repos/git/git.svg?fullname=)](https://github.com/git/git){target=_blank}

## Configuration in MegaLinter

- Enable git_diff by adding `GIT_GIT_DIFF` in [ENABLE_LINTERS variable](https://megalinter.github.io/configuration/#activation-and-deactivation)
- Disable git_diff by adding `GIT_GIT_DIFF` in [DISABLE_LINTERS variable](https://megalinter.github.io/configuration/#activation-and-deactivation)

| Variable                                 | Description                                                                                                                                                                                  | Default value      |
|------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------|
| GIT_GIT_DIFF_ARGUMENTS                   | User custom arguments to add in linter CLI call<br/>Ex: `-s --foo "bar"`                                                                                                                     |                    |
| GIT_GIT_DIFF_FILE_EXTENSIONS             | Allowed file extensions. `"*"` matches any extension, `""` matches empty extension. Empty list excludes all files<br/>Ex: `[".py", ""]`                                                      | Exclude every file |
| GIT_GIT_DIFF_FILE_NAMES_REGEX            | File name regex filters. Regular expression list for filtering files by their base names using regex full match. Empty list includes all files<br/>Ex: `["Dockerfile(-.+)?", "Jenkinsfile"]` | Include every file |
| GIT_GIT_DIFF_PRE_COMMANDS                | List of bash commands to run before the linter                                                                                                                                               | None               |
| GIT_GIT_DIFF_POST_COMMANDS               | List of bash commands to run after the linter                                                                                                                                                | None               |
| GIT_GIT_DIFF_DISABLE_ERRORS              | Run linter but consider errors as warnings                                                                                                                                                   | `false`            |
| GIT_GIT_DIFF_DISABLE_ERRORS_IF_LESS_THAN | Maximum number of errors allowed                                                                                                                                                             | `0`                |

## MegaLinter Flavours

This linter is available in the following flavours

|                                                                         <!-- -->                                                                         | Flavor                                                               | Description                                                            | Embedded linters |                                                                                                                                                                                                 Info |
|:--------------------------------------------------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------|:-----------------------------------------------------------------------|:----------------:|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| <img src="https://github.com/megalinter/megalinter/raw/main/docs/assets/images/mega-linter-square.png" alt="" height="32px" class="megalinter-icon"></a> | [all](https://megalinter.github.io/supported-linters/)               | Default MegaLinter Flavor                                              |        97        |                             ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/megalinter/megalinter/v5) ![Docker Pulls](https://img.shields.io/docker/pulls/megalinter/megalinter) |
|      <img src="https://github.com/megalinter/megalinter/raw/main/docs/assets/icons/ci_light.ico" alt="" height="32px" class="megalinter-icon"></a>       | [ci_light](https://megalinter.github.io/flavors/ci_light/)           | Optimized for CI items (Dockerfile, Jenkinsfile, JSON/YAML schemas,XML |        16        |           ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/megalinter/megalinter-ci_light/v5) ![Docker Pulls](https://img.shields.io/docker/pulls/megalinter/megalinter-ci_light) |
|        <img src="https://github.com/megalinter/megalinter/raw/main/docs/assets/icons/dart.ico" alt="" height="32px" class="megalinter-icon"></a>         | [dart](https://megalinter.github.io/flavors/dart/)                   | Optimized for DART based projects                                      |        42        |                   ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/megalinter/megalinter-dart/v5) ![Docker Pulls](https://img.shields.io/docker/pulls/megalinter/megalinter-dart) |
|    <img src="https://github.com/megalinter/megalinter/raw/main/docs/assets/icons/documentation.ico" alt="" height="32px" class="megalinter-icon"></a>    | [documentation](https://megalinter.github.io/flavors/documentation/) | MegaLinter for documentation projects                                  |        41        | ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/megalinter/megalinter-documentation/v5) ![Docker Pulls](https://img.shields.io/docker/pulls/megalinter/megalinter-documentation) |
|       <img src="https://github.com/megalinter/megalinter/raw/main/docs/assets/icons/dotnet.ico" alt="" height="32px" class="megalinter-icon"></a>        | [dotnet](https://megalinter.github.io/flavors/dotnet/)               | Optimized for C, C++, C# or VB based projects                          |        48        |               ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/megalinter/megalinter-dotnet/v5) ![Docker Pulls](https://img.shields.io/docker/pulls/megalinter/megalinter-dotnet) |
|         <img src="https://github.com/megalinter/megalinter/raw/main/docs/assets/icons/go.ico" alt="" height="32px" class="megalinter-icon"></a>          | [go](https://megalinter.github.io/flavors/go/)                       | Optimized for GO based projects                                        |        43        |                       ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/megalinter/megalinter-go/v5) ![Docker Pulls](https://img.shields.io/docker/pulls/megalinter/megalinter-go) |
|        <img src="https://github.com/megalinter/megalinter/raw/main/docs/assets/icons/java.ico" alt="" height="32px" class="megalinter-icon"></a>         | [java](https://megalinter.github.io/flavors/java/)                   | Optimized for JAVA based projects                                      |        43        |                   ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/megalinter/megalinter-java/v5) ![Docker Pulls](https://img.shields.io/docker/pulls/megalinter/megalinter-java) |
|     <img src="https://github.com/megalinter/megalinter/raw/main/docs/assets/icons/javascript.ico" alt="" height="32px" class="megalinter-icon"></a>      | [javascript](https://megalinter.github.io/flavors/javascript/)       | Optimized for JAVASCRIPT or TYPESCRIPT based projects                  |        50        |       ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/megalinter/megalinter-javascript/v5) ![Docker Pulls](https://img.shields.io/docker/pulls/megalinter/megalinter-javascript) |
|         <img src="https://github.com/megalinter/megalinter/raw/main/docs/assets/icons/php.ico" alt="" height="32px" class="megalinter-icon"></a>         | [php](https://megalinter.github.io/flavors/php/)                     | Optimized for PHP based projects                                       |        46        |                     ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/megalinter/megalinter-php/v5) ![Docker Pulls](https://img.shields.io/docker/pulls/megalinter/megalinter-php) |
|       <img src="https://github.com/megalinter/megalinter/raw/main/docs/assets/icons/python.ico" alt="" height="32px" class="megalinter-icon"></a>        | [python](https://megalinter.github.io/flavors/python/)               | Optimized for PYTHON based projects                                    |        49        |               ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/megalinter/megalinter-python/v5) ![Docker Pulls](https://img.shields.io/docker/pulls/megalinter/megalinter-python) |
|        <img src="https://github.com/megalinter/megalinter/raw/main/docs/assets/icons/ruby.ico" alt="" height="32px" class="megalinter-icon"></a>         | [ruby](https://megalinter.github.io/flavors/ruby/)                   | Optimized for RUBY based projects                                      |        42        |                   ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/megalinter/megalinter-ruby/v5) ![Docker Pulls](https://img.shields.io/docker/pulls/megalinter/megalinter-ruby) |
|        <img src="https://github.com/megalinter/megalinter/raw/main/docs/assets/icons/rust.ico" alt="" height="32px" class="megalinter-icon"></a>         | [rust](https://megalinter.github.io/flavors/rust/)                   | Optimized for RUST based projects                                      |        42        |                   ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/megalinter/megalinter-rust/v5) ![Docker Pulls](https://img.shields.io/docker/pulls/megalinter/megalinter-rust) |
|     <img src="https://github.com/megalinter/megalinter/raw/main/docs/assets/icons/salesforce.ico" alt="" height="32px" class="megalinter-icon"></a>      | [salesforce](https://megalinter.github.io/flavors/salesforce/)       | Optimized for Salesforce based projects                                |        44        |       ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/megalinter/megalinter-salesforce/v5) ![Docker Pulls](https://img.shields.io/docker/pulls/megalinter/megalinter-salesforce) |
|        <img src="https://github.com/megalinter/megalinter/raw/main/docs/assets/icons/scala.ico" alt="" height="32px" class="megalinter-icon"></a>        | [scala](https://megalinter.github.io/flavors/scala/)                 | Optimized for SCALA based projects                                     |        42        |                 ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/megalinter/megalinter-scala/v5) ![Docker Pulls](https://img.shields.io/docker/pulls/megalinter/megalinter-scala) |
|        <img src="https://github.com/megalinter/megalinter/raw/main/docs/assets/icons/swift.ico" alt="" height="32px" class="megalinter-icon"></a>        | [swift](https://megalinter.github.io/flavors/swift/)                 | Optimized for SWIFT based projects                                     |        42        |                 ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/megalinter/megalinter-swift/v5) ![Docker Pulls](https://img.shields.io/docker/pulls/megalinter/megalinter-swift) |
|      <img src="https://github.com/megalinter/megalinter/raw/main/docs/assets/icons/terraform.ico" alt="" height="32px" class="megalinter-icon"></a>      | [terraform](https://megalinter.github.io/flavors/terraform/)         | Optimized for TERRAFORM based projects                                 |        47        |         ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/megalinter/megalinter-terraform/v5) ![Docker Pulls](https://img.shields.io/docker/pulls/megalinter/megalinter-terraform) |

## Behind the scenes

### How are identified applicable files

- If this linter is active, all files will always be linted

<!-- markdownlint-disable -->
<!-- /* cSpell:disable */ -->
### How the linting is performed

git_diff is called once on the whole project directory

- filtering can not be done using MegaLinter configuration variables,it must be done using git_diff configuration or ignore file (if existing)
- `VALIDATE_ALL_CODEBASE: false` does not make git_diff analyze only updated files

### Example calls

```shell
git diff --check
```


### Help content

```shell
usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]

These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
   clone             Clone a repository into a new directory
   init              Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
   add               Add file contents to the index
   mv                Move or rename a file, a directory, or a symlink
   restore           Restore working tree files
   rm                Remove files from the working tree and from the index
   sparse-checkout   Initialize and modify the sparse-checkout

examine the history and state (see also: git help revisions)
   bisect            Use binary search to find the commit that introduced a bug
   diff              Show changes between commits, commit and working tree, etc
   grep              Print lines matching a pattern
   log               Show commit logs
   show              Show various types of objects
   status            Show the working tree status

grow, mark and tweak your common history
   branch            List, create, or delete branches
   commit            Record changes to the repository
   merge             Join two or more development histories together
   rebase            Reapply commits on top of another base tip
   reset             Reset current HEAD to the specified state
   switch            Switch branches
   tag               Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch             Download objects and refs from another repository
   pull              Fetch from and integrate with another repository or a local branch
   push              Update remote refs along with associated objects

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.
See 'git help git' for an overview of the system.
```

### Installation on mega-linter Docker image


### Example success log

```shell
Results of git_diff linter (version 2.26.2)
See documentation on https://megalinter.github.io/descriptors/git_git_diff/
-----------------------------------------------

[SUCCESS] .automation/test/git_diff/good
    

```