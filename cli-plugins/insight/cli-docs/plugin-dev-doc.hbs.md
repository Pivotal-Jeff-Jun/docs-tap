# Plugin dev docs

## Directory Structure

artifacts/: Where you plugins build output will be located

Makefile: Makefile for the plugin

cmd/plugin/< plug-in >: Path where plugins main directory will live

cmd/plugin/< plug-in >/test: Plugins are required to have a test command defined

## Commands

`make build`: builds your plugin artifacts

`make lint`: run the golangci linter on your plugin code

`make build-install-local`: locally build, publish, and install plugin

## Scripts

These dev scripts are located under `scripts/dev/`

`delete-tanzu.sh`: delete tanzu cli and plugins installed locally

`install-tanzu.sh`: clean installation of tanzu cli
* running `install-tanzu.sh` will install latest tanzu framework with latest builder plugin
* running `install-tanzu.sh <path-to-tanzu-framework-tarball>` will install the specified tanzu framework tarball