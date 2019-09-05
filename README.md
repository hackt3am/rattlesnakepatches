build config for rattlesnake os:

[[custom-patches]]
  repo = "https://github.com/madelponte/rattlesnakepatches"
  patches = [
  "0001-opengapps-walleye.patch",
  "0002-global-internet-permission-toggle.patch",
  "0003-global-sensors-permission-toggle.patch",
  "0004-enable-doze.patch"
]

[[custom-scripts]]
  repo = "https://github.com/madelponte/rattlesnakescripts"
  scripts = [ "0001-opengapps-dependencies.sh" ]

[[custom-manifest-remotes]]
  name = "opengapps"
  fetch = "https://github.com/opengapps/"
  revision = "master"

[[custom-manifest-remotes]]
  name = "gitlab"
  fetch = "https://gitlab.opengapps.org/opengapps/"
  revision = "master"

[[custom-manifest-projects]]
  path = "vendor/opengapps/build"
  name = "aosp_build"
  remote = "opengapps"

[[custom-manifest-projects]]
  path = "vendor/opengapps/sources/all"
  name = "all"
  remote = "gitlab"

[[custom-manifest-projects]]
  path = "vendor/opengapps/sources/arm"
  name = "arm"
  remote = "gitlab"

[[custom-manifest-projects]]
  path = "vendor/opengapps/sources/arm64"
  name = "arm64"
  remote = "gitlab"

[[custom-manifest-projects]]
  path = "vendor/opengapps/sources/x86"
  name = "x86"
  remote = "gitlab"

[[custom-manifest-projects]]
  path = "vendor/opengapps/sources/x86_64"
  name = "x86_64"
  remote = "gitlab"


