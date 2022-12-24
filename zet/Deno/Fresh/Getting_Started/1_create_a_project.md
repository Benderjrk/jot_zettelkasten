# Create A Project

New Fresh projects can be created by using the fresh project creation
tool. It will scaffold out a new project with some examples files to get
you started.

The create a new project, run:

```bash
deno run -A -r https://fresh.deno.dev my-project
cd my-project
deno task start
```

This will scaffold out the new project, then switch into the newly created directory, and then start the development server.

This will create a directory containing some files and directories. There are 4 files that are strictly necessary to run a fresh project:

* `dev.ts`: This is the development entry point for your project. This is the file that you run to start your project. This file doesn't need to be called `dev.ts`, but this is the convention.
* `main.ts`: This is the production entry point for your project. It is the file tat you link to Deno Deploy. This file doesn't actually need to be `main.ts`, but this is the convention.
* `fresh.gen.ts`: This is the manifest file that contains information about your routes and islands. This file is automatically generated in development based on your `routes/` and `islands/` folders.
* `import_map.json`: This is an import map that is used to manage dependencies for the project. This allows for easy importing and updating of dependencies.

---

A `deno.json` file is also created in the project directory. This file does two things:

* It tells Deno about the location of the import map, so that it can be loaded automatically.
* It registers a "start" task to run the project without having to type a long `deno run` command.

Two important folders are also created that contain your routes and islands respectively:

* `routes/`: This folder contains all of the routes in your project. The names of each file in this folder correspond to the path where the page will be accessed. Code inside of this folder is never directly shipped to the client. You'll learn more about how routes work in the next section.
* `islands/`: This folder contains all of the interactive islands in your project. The name of each file corresponds to the name of the island defined in that file. Code inside of this folder can be run from both client and server. You'll learn more about islands later in this chapter.

Finally a `static/` folder is created that contains static files that are automatically served "as is".
