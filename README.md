# silverstripe framework errorpage patch

## Maintainers

 * Andre Lohmann (Nickname: andrelohmann)
  <lohmann dot andre at googlemail dot com>

## Requirements

Silverstripe 3.2.*

## Introduction

Patches silverstripe framework core to create custom error pages when cms-module not in use.

## Installation

always install the Version number matching your silverstripe framework version

put the follwoing post install and post updates scripts into your composer.json

```

    "scripts": {
        "post-install-cmd": [
            "cp vendor/andrelohmann-silverstripe/framework-errorpage-patch/* -r framework/"
        ],
        "post-update-cmd": [
            "cp vendor/andrelohmann-silverstripe/framework-errorpage-patch/* -r framework/"
        ]
    },

## Usage

create following files:

```
/YOURPROJECTFOLDER/templates/ErrorPage.ss
/YOURPROJECTFOLDER/templates/Layout/ErrorPage.ss
```

These Files will build your custom Error Page

