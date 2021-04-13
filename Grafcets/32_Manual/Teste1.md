<img src="https://github.com/LMigu3liPT/Documentation_Luban/blob/main/Grafcets/32_Manual/Imagens_Grafcets/Logo_Luban.png" width="80" />    

# Lu ban Workshop Portugal

This PHP library provide the functionality to automatic create a new tag/version in a remote VCS repository dependending on the last created tag/version. It follows the semantic versioning pattern: http://semver.org/
You are be able configure the version type to increase. For example "major" or "minor" increasement.

Features:
 - Follows the semantic versioning pattern
 - Major, minor and patch version are supported
 - GIT integration
 - Commit (and push) additional files before creating a new tag/version
 - Dry run. Just evaluate the next tag/version

## Index
- [Installation](#installation)
  - [Clone](#clone)
  - [Composer](#composer)
- [Usage](#usage)
  - [Version-Type](#version-type)
  - [Commit files before creating a new tag/version](#commit-files-before-creating-a-new-tagversion)
  - [Evaluate (dry run)](#evaluate-dry-run)

## Installation
This library is build with composer. So you can even clone this repisory and install the dependencies via composer or just require this library in the composer.json of your project.

### Clone
clone the repitory from GitHub

    git clone https://github.com/AOEpeople/Tagging.git .

and install dependencies via composer

    wget http://getcomposer.org/composer.phar
    php composer.phar install

