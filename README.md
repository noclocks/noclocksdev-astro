# No Clocks, LLC Website (Astro)

> [!NOTE]
> *This is a work in progress. The website is currently being developed, transitioning from the legacy site to a new Astro implementation.*

## Purpose

This repository contains the source for the upcoming No Clocks, LLC website.
It is built with [Astro](https://astro.build) and showcases the company's services,
technology expertise, team, and contact information.

## Project Structure

The project follows a standard Astro structure with these key directories:

- `src/` - Source code including components, layouts, pages, and styles
- `public/` - Static assets like images and fonts
- `docs/` - Documentation and project information
- `legacy/noclocks.dev/` - Previous website version with extracted HTML/JS/styles/images used as reference

## Getting Started

Install the project dependencies once you have cloned the repository:

```sh
npm install
```

## Development Server

To start a local development server with live reload, run:

```sh
npm run dev
```

## Production Build

Generate a production build in the `dist` directory with:

```sh
npm run build
```

## Legacy Website Reference

The original website has been extracted and stored in the `legacy/noclocks.dev/` directory.
This serves as a reference for content, design, and functionality when implementing
features in the new Astro site. Do not modify these files, as they are for reference only.

## Current Pages

The following pages are being implemented in the new Astro site:

- Homepage
- About
- Services
- Team
- Contact

## Large Files

Large binaries such as legacy archives or high-resolution screenshots are tracked with
[Git LFS](https://git-lfs.com/) or kept outside the repository.

```shell
git lfs track "legacy/legacy-b12.zip"
```
