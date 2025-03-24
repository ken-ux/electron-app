# electron-app

This is a simple desktop application that displays the user's Chrome, Node.js, and Electron versions and has a toggle for a dark mode appearance. It follows the Electron tutorials for [Building your First App](https://www.electronjs.org/docs/latest/tutorial/tutorial-first-app) and example for implementing [Dark Mode](https://www.electronjs.org/docs/latest/tutorial/dark-mode). It slightly deviates from the tutorials by using ECMAScript modules instead of CommonJS for its imports and exports.

## Getting Started

You can download the source code and run this application locally.

### Installation and Usage

1. Clone the repo

```
git clone git@github.com:ken-ux/electron-app.git
```

2. Install the packages

```
npm install
```

3. Run the start script to open the app

```
npm run start
```

## Lessons Learned

- `import.meta.dirname` can be used in ECMAScript modules for newer versions of Node (20.11/21.2+) to reference the directory name of the module. It is identical in functionality to `__dirname`, which is used in older versions.
- Communicating between the `main` and `renderer` processes using the inter-process communication documentation from Electron.
- Understanding how to integrate operating system settings, such as native theme, into Electron apps.
- Packaging Electron apps to create distributables that can run on different operating systems.
