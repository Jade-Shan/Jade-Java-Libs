Jade-Java-libs
======================

Base pom for all my java project. Defines:

* all libs and version
* rule for unit test class name
* scop dependencies
* remote maven repository

Config
----------------------

### Unit Test Rules

inclues:

* `**/*Test.java`
* `**/*Spec.java`
* `**/UnitTestSuite.java`

excludes:

* `**/Abstract*.java`
* `**/*IntegrationTest.java`
* `**/*Tests.java`

### Deploy by profile

Pre-define 4 profiles:

#### `dev` for developing

#### `prd` for online production env

#### `dpl` for deploy in private maven repo 

Compile scope and runtime scope is provided for save space in 
private maven server.

#### `rls` for deploy in oss.sonatype.org maven repo

Set maven server to oss.sonatype.org



change log
=========================

## 1.0.14

* :heavy_plus_sign: add jsr-250 java-annotation-api

* :arrow_up: mysql-connection-j update to 8.0.19
* :arrow_up: jackson-databind.version update to 2.9.10.4

## 1.0.13

* :arrow_up: javamail version update version from 1.4.1 to 1.4.7
* :arrow_up: greenmail version update version from 1.5.9
* :arrow_up: jackson-databing version update version 2.9.9

* :heavy_plus_sign: add fastjson 1.2.58

* :pencil2: remove duplicate declaration of slf4j


## 1.0.12

* :heavy_plus_sign: javamelody update version 1.75.0

## 1.0.11

* :fire: remove profile filter file from base profile
* :wrench: change sqlite jdbc driver maven dependency from test-scop to compile-scop

add lib:

* :heavy_plus_sign: hamcrest-all
* :heavy_plus_sign: dd-plist
* :heavy_plus_sign: jackson-databind
* :heavy_plus_sign: commons-lang3
* :heavy_plus_sign: slf4j-api
* :heavy_plus_sign: slf4j-simple
* :heavy_plus_sign: slf4j-jdk14

update lib version:

* :arrow_up: jopt-simple
* :arrow_up: jackson-mapper-asl
* :arrow_up: jsoup
* :arrow_up: slf4j
* :arrow_up: sqlite-jdbc
* :arrow_up: commons-fileupload update version 1.3.3
* :arrow_up: spring update version 4.3.21.RELEASE

## 1.0.10

* :heavy_plus_sign: add hikaricp as JDBC Connection Pool framework
* :heavy_plus_sign: add slf4j-log4j12
* :heavy_plus_sign: add slf4j-simple
* :heavy_plus_sign: add junit-interface
* :heavy_plus_sign: add javamelody
* :wrench: change junit test case postfix: add `**/*Spec.java`

提交说明
=====================

developing

* :tada:                      `:tada:`                     Initial commit.
* :construction:              `:construction:`             Work in progress.
* :hankey:                    `:hankey:`                   Writing bad code that needs to be improved.
* :sparkles:                  `:sparkles:`                 Introducing new features.
* :lipstick:                  `:lipstick:`                 Updating the UI and style files.
* :zap:                       `:zap:`                      Improving performance.
* :alien:                     `:alien:`                    Updating code due to external API changes.
* :rewind:                    `:rewind:`                   Reverting changes.

testing

* :white_check_mark:          `:white_check_mark:`         Adding tests.
* :chart_with_upwards_trend:  `:chart_with_upwards_trend:` Adding analytics or tracking code(Performance).
* :paw_prints:                `:paw_prints:`               Adding analytics or tracking code(Logic).

refactor

* :art:                       `:art:`                      Improving structure / format of the code.
* :truck:                     `:truck:`                    Moving or renaming files.
* :fire:                      `:fire:`                     Removing code or files.
* :hammer:                    `:hammer:`                   Heavy refactoring.

bugfix

* :pencil2:                   `:pencil2:`                  Fixing typos.
* :rotating_light:            `:rotating_light:`           Removing linter warnings.
* :bug:                       `:bug:`                      Fixing a bug.
* :lock:                      `:lock:`                     Fixing security issues.
* :ambulance:                 `:ambulance:`                Critical hotfix.

configuration

* :wrench:                    `:wrench:`                   Changing configuration files.
* :globe_with_meridians:      `:globe_with_meridians:`     Internationalization and localization.
* :package:                   `:package:`                  Updating compiled files or packages.
* :heavy_plus_sign:           `:heavy_plus_sign:`          Adding a dependency.
* :heavy_minus_sign:          `:heavy_minus_sign:`         Removing a dependency.
* :arrow_up:                  `:arrow_up:`                 Upgrading dependencies.
* :arrow_down:                `:arrow_down:`               Downgrading dependencies.

documents

* :pencil:                    `:pencil:`                   Comments in code.
:qa

* :memo:                      `:memo:`                     Writing docs.
* :page_facing_up:            `:page_facing_up:`           Adding or updating license.

version

* :bookmark:                  `:bookmark:`                 Releasing / Version tags.
* :twisted_rightwards_arrows: `:twisted_rightwards_arrows:`Merging branches.

deploy

* :construction_worker:       `:construction_worker:`      Adding CI build system.
* :green_heart:               `:green_heart:`              Fixing CI Build.
* :rocket:                    `:rocket:`                   Deploying stuff.

plantform

* :apple:                     `:apple:`                    Fixing something on macOS.
* :penguin:                   `:penguin:`                  Fixing something on Linux.
* :checkered_flag:            `:checkered_flag:`           Fixing something on Windows.
* :whale:                     `:whale:`                    Work about Docker.


