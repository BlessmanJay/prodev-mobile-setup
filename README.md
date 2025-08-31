# Setting Up The Mobile Development Environment

## Installations

The following were installed:

Node.js (v22.15.1) Expo CLI, using (npm install -g expo-cli)

A code editor (VS Code)

Also, Expo Go was downloaded, installed, and set up on my physical device.

No errors encountered and no challenges faced during the installation phase.

## Resetting the Project

This project includes a script to reset the environment and re-scaffold dependencies from scratch using:

npm run reset-project

### What Happens During Reset

When you run the command above, the following steps are executed:

First, a message pops up in the Terminal which reads below:

Do you want to move existing files to /app-example instead of deleting them? (Y/n):

On pressing the 'Enter' key, the following took place.

#### 1. Delete existing dependencies

The node_modules/ folder is removed.

The package-lock.json file is deleted (to avoid conflicts and ensure fresh dependency resolution).

#### 2. Reinstall dependencies

A clean npm install is triggered, which re-downloads all packages listed in package.json.

A new package-lock.json file is generated with the latest resolved versions.

#### 3. Re-scaffold project (if applicable)

Any scaffolding scripts (for example, setting up configs, environment files, or project boilerplate) are re-applied.

This ensures the project structure and configuration return to their default state.

### Observations

- Running npm run reset-project is helpful when encountering dependency errors or corrupted installs.

- It guarantees the project is rebuilt from a clean slate, just like when first cloned from the repository.

- The process can take a few minutes since all dependencies are freshly downloaded.

- After reset, you can continue development by starting the dev server:
  npm run dev
