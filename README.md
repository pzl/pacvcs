PacVCS
======

`pacvcs` is a script that checks how far out of date your currently-installed VCS-based packages are with their upstream counterparts. 

The output is color-coded to give easy status information at a glance. A green package title means your currently installed version matches the remote. Red means you are verifiably out of date. Yellow means there was a problem fetching or determining the remote version (check the provided URL?) and the script cannot determine if you're out of date.

The script is most heavily tested on git- and github-based repositories, but should work with other packages using gitlab, sourceforge, launchpad, etc.

You may need to edit your PKGBUILDs before installation to make sure the URL of the package may not be the person-friendly project homepage, but instead points to the VCS project itself. E.g. Change it from "http://my-awesome-project.github.com/intro" to "https://github.com/author/my-awesome-project.git"


Examples
--------

Here are some URL formats that will work with pacvcs:

- `git://github.com/signal11/hidapi`
- `https://github.com/chjj/compton`
- `lp:kicad`
- `git://git.code.sf.net/p/openocd/code`
- `https://gitlab.com/o9000/tint2.git`


