# ROS 2 + PX4 Dev Guide

A self-contained reference for building a ROS 2 (Jazzy) workspace against PX4
SITL. It uses [pixi](https://pixi.sh) for the environment and
[basedpyright](https://docs.basedpyright.com) for Python type checking, so no
system-level ROS install is needed.

The site is built with [Quarto](https://quarto.org) and deployed to GitHub
Pages on every push to `main`:

**<https://riccardo.github.io/ros2-px4-docs>**

## What's inside

- **Setup** -- workspace, PX4 SITL, uXRCE-DDS agent, C++ and bringup packages, one-command launch
- **Tooling** -- basedpyright, clangd, testing
- **Control** -- QoS profiles, control loop, node composition, parameters, frame conventions, arming/offboard, low-level control, control allocation

## Build locally

```bash
quarto preview   # live-reloading server
quarto render    # static build into _site/
```

## Layout

```
index.qmd     Landing page
_quarto.yml   Site config (navbar, sidebar, theme)
docs/         Guides, grouped under setup/ tooling/ control/
themes/       stream light/dark SCSS themes
```