# ROS 2 + PX4 Dev Guide

A self-contained reference for setting up a ROS 2 (Jazzy) workspace targeting
PX4 SITL, using [pixi](https://pixi.sh) as the environment manager and
[basedpyright](https://docs.basedpyright.com) for Python type checking. No
system-level ROS install required.

Built with [Quarto](https://quarto.org) and published to GitHub Pages on every
push to `main`.

## Contents

- **Setup** -- workspace, PX4 SITL, uXRCE-DDS agent, C++/bringup packages, one-command launch
- **Tooling** -- basedpyright, clangd, testing
- **Control** -- QoS profiles, control loop, node composition, parameters, frame conventions, arming/offboard, low-level control, control allocation

## Building locally

```bash
quarto preview   # live-reloading local server
quarto render    # static build into _site/
```

## Layout

```
index.qmd        Landing page
_quarto.yml      Site config (navbar, sidebar, theme)
docs/            Guides, grouped by setup/ tooling/ control/
themes/          stream light/dark SCSS themes
```
