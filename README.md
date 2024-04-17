![](./.github/repo-banner.png)

# Mastering 3D Web Development with TresJS ecosystem - A Vue.js Workshop

This repository contains the source code for the Vue.js workshop on mastering 3D web development with the TresJS ecosystem for [Vue.js Live 2024](https://vuejslive.com/).

## Usage

### Install dependencies

This repository provides a `pnpm workspace` setup. Please make sure you have `pnpm` installed on your machine. Check how here: [pnpm installation](https://pnpm.io/installation).

```bash
npm install -g pnpm
```

To install the dependencies, run the following command:

```bash
pnpm install
```

### Run excersices

Each exercise is located in a separate project inside `excercises` folder. 

0. Starter [./exercises/starter](./exercises/starter): This is the starting point for the workshop. It contains a basic Vue.js project with TresJS and Vite installed.

1. Basic Scene [./exercises/basic-scene](./exercises/basic-scene)
2. Perspective Camera [./exercises/camera](./exercises/camera)
3. Geometries [./exercises/geometries](./exercises/geometries)
4. Materials [./exercises/materials](./exercises/materials)
5. Lights & Shadows [./exercises/lights-shadows](./exercises/lights-shadows)
6. Renderloop [./exercises/animate-loop](./exercises/animate-loop)
7. Primitives [./exercises/primitives](./exercises/primitives)
8. Models [./exercises/models](./exercises/models)


To run an exercise, navigate to the exercise folder and run the following command:

```bash
pnpm run dev
```

