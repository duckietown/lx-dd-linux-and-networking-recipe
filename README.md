<p align="center">
<a href="https://duckietown.com"><img src="https://raw.githubusercontent.com/duckietown/lx-dd-linux-and-networking/ente/assets/images/dtlogo.png" alt="Duckietown Logo" width="50%"></a>
</p>

# Recipe: Linux and Networking LX

This is the recipe for the [`lx-dd-linux-and-networking`](https://github.com/duckietown/lx-dd-linux-and-networking)
Learning Experience. It holds everything the learner never sees: the Docker images, the
dependencies, and the launcher.

Learners do not clone this repository. The Duckietown Shell pulls it automatically, because
`lx-dd-linux-and-networking/.dtproject` points at it:

    RECIPE_REPOSITORY=duckietown/lx-dd-linux-and-networking-recipe
    RECIPE_BRANCH=ente

## What is here

| Path | Purpose |
| --- | --- |
| `Dockerfile` | image that runs the LX code on a Duckiedrone |
| `Dockerfile.vscode` | image behind `dts code editor`, the browser editor the learner works in |
| `dependencies-apt.txt`, `dependencies-py3.txt` | packages installed into those images |
| `dependencies-apt.vscode.txt` | extra APT packages for the editor image only |
| `launchers/default.sh` | what runs when the LX container starts |
| `settings.yaml` | Duckiematrix map and vehicle used by `dts code start_matrix` |
| `assets/vscode/setup.sh` | code-server tweaks (open the README, enable Jupyter widgets) |
| `packages/` | instructor-only code, hidden from the learner |
