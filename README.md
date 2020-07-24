# SBo-management
slackbuild packaging tool

A shell script for automate the process of building 
Slackware packages from slackbuilds.org

Usage: slackbuild-management.sh search|indo|download|pack|install packagename
  search - search for a package
  download - download the package files
  pack - download and build the SlackBuilds
  info - shows the SlackBuilds info
 * update - updates local SlackBuilds index


 
Building enviroment variables:
 - TMP_DIR : Changes the temp folder
 - SBo_OUTPUT : where to save the output package, defaults (/tmp). If declared,
the package category is appended. For example:
# SBo_OUTPUT=/mnt/localbuilds ./slackbuild-management.sh pack colordiff
Generates the following output:
# Slackware package /mnt/localbuilds/./development/colordiff-1.0.15-noarch-1_SBo.tgz created.

 - ADDON : any additional parameters passed to PRGNAM.SlackBuild
