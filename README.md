# ReVanced Builder
[![CI](https://github.com/moreorlessanand/revanced-builder/actions/workflows/ci.yml/badge.svg?event=schedule)](https://github.com/moreorlessanand/revanced-builder/actions/workflows/ci.yml)

Extensive ReVanced builder  

Get the [latest CI release](https://github.com/moreorlessanand/revanced-builder/releases).

<details><summary><big>Features</big></summary>
<ul>
 <li>Support all present and future ReVanced and <a href="https://github.com/inotia00/revanced-patches">ReVanced Extended</a> apps</li>
 <li> Can build non-root APKs</li>
 <li> Updated daily with the latest versions of apps and patches</li>
 <li> Optimize APKs and modules for size</li>
 <li> Modules</li>
    <ul>
     <li> recompile invalidated odex for faster usage</li>
     <li> handle installation of the correct version of the stock app and all that</li>
    </ul>
</ul>
Note that the <a href="../../actions/workflows/ci.yml">CI workflow</a> is scheduled to build the modules and APKs everyday using GitHub Actions if there is a change in ReVanced patches. You may want to disable it.
</details>

## To include/exclude patches or patch other apps

 * Star the repo :eyes:
 * Use the repo as a [template](https://github.com/new?template_name=revanced-builder&template_owner=moreorlessanand)
 * Customize [`config.toml`](./config.toml) using [rvmm-config-gen](https://j-hc.github.io/rvmm-config-gen/)
 * Run the build [workflow](../../actions/workflows/build.yml)
 * Grab your modules and APKs from [releases](../../releases)

also see here [`CONFIG.md`](./CONFIG.md)

## Building Locally
### On Termux
```console
bash <(curl -sSf https://raw.githubusercontent.com/moreorlessanand/revanced-builder/main/build-termux.sh)
```

### On Desktop
```console
$ git clone https://github.com/moreorlessanand/revanced-builder
$ cd revanced-magisk-module
$ ./build.sh
```
