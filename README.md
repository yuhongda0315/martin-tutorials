# RongCloud tutorials

## Running this site

There are two primary ways to run this website locally. We recommend using the `./run` command, which runs the site through Docker. The site can also run directly on the system with our build tools and Polymer.


### `./run` command

We also make use of a `./run` script that we generate with our [generator-canonical-webteam Yeoman generator](https://github.com/canonical-webteam/generator-canonical-webteam).

#### Dependencies

- Latest version of Docker


#### Usage

- `./run`: Run local server with example content.
- `./run serve [file or folder]`: Run server and watch a local file or folder.
- `./run help`: Print help.

NPM/Yarn scripts:
- `./run exec yarn run serve-live`: Run local server with live content.
- `./run exec yarn run build-all`: Generate live tutorials and build live site.
- `./run exec yarn run build-site`: Build site to `build` folder.
- `./run exec yarn run build-tutorials`: Generate live tutorials.
- `./run exec yarn run start-server`: Start sever with production config.
- `./run exec yarn run polymer [args]`: Run a command through Polymer.


### Running without Docker

#### Dependencies

- Yarn or NPM
- Bower

(`npm` can be used in place of `yarn` in this document.)

Install NPM and Bower dependencies:
``` bash
$ yarn install
$ bower install
```


#### Quick start

Start up a local server which watches the `examples` folder:

``` bash
$ yarn run serve ./examples
```

The `./examples` in the command can be replaced with another path.


#### Usage

Scripts are set up through the `package.json` file and run through Yarn:

- `yarn run serve [file or folder]`: Run server and watch a local file or folder.
- `yarn run build`: Generate Tutorials and build live site.
- `yarn run serve-live`: Run local server with live content.
- `yarn run build-site`: Build site to `build` folder.
- `yarn run build-tutorials`: Generate live tutorials.
- `yarn run start-server`: Generate live tutorials.
- `yarn run polymer [args]`: Run a command through Polymer.


## Building Your Application

Running the build command will generate a `build/` folder with `bundled/` and `unbundled/` sub-folders containing bundled (Vulcanized) and unbundled builds. These builds are run through HTML, CSS, and JS optimizers.


## Contributor

[https://github.com/canonical-web-and-design/tutorials.ubuntu.com](https://github.com/canonical-web-and-design/tutorials.ubuntu.com)

