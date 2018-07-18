**[Join KCauldron's Discord!]~~(https://discord.gg/0nuu0DLm3WJq1Z23)~~**
# KCauldron
### UKCauldron - continuation of KCauldron and Cauldron Minecraft server

## Building UKCauldron
* Ensure you are using Java JDK 8u101 or higher.
* Checkout project
  * You can use your IDE or clone from Git:
  `git clone ${url}`
* Init submodules
  * Since this project is a merger of two others, we need both.
  `git submodule update --init --recursive`
* Setup initial workspace
  * This process will download Minecraft and apply patches
  * If you have Gradle integration in your IDE - you can still use GUI
  `./gradlew setupCauldron` or `gradlew.bat setupCauldron`
* Build both legacy server jar & default jar
  `./gradlew jar` or `gradlew.bat jar`

## Updating sources
If you have once checked out the source - you do not need to do it again.
* Update sources
  * `git pull origin master`
* Reapply patches & build binaries
  * `./gradlew clean setupCauldron jar`


## Submitting Issues
* First check the bug in single player and vanilla Forge, if the bug is still present - mod issue
* Check with minimal server environment
  * Remove all unnecessary plugins and mods
  * Reset all configs to default
  If the bug is still present - mod compatibility issue
* If you're using beta-release of UKCauldron - check the latest stable version
  * All versions situated ~~(https://repo.prok.pw/pw/prok/KCauldron/?C=M&O=D)~~
* If the bug is still present - UKCauldron issue
  * Make sure that a similar issue does not exist already
  * Please fill ~~(https://gitlab.prok.pw/Prototik/KCauldron/issues/new)~~.