# Jekyll Example

[![Built with Devbox](https://jetpack.io/devbox/img/shield_moon.svg)](https://jetpack.io/devbox/docs/contributor-quickstart/)

Inspired by https://litchipi.github.io/nix/2023/01/12/build-jekyll-blog-with-nix.html 

## How to Use

1. Install [Devbox](https://www.jetpack.io/devbox/docs/installing_devbox/)
2. Run `devbox shell` to install your packages and run the init hook
3. In the root directory, run `devbox run generate` to install and package the project with bundler
4. In the root directory, run `devbox run server` to start the server. You can access the Jekyll example at `localhost:4000`

## How to Create this Example from Scratch

1. Install [Devbox](https://www.jetpack.io/devbox/docs/installing_devbox/)
1. In a new directory, run `devbox init` to create an empty config
1. Run `devbox add ruby_3_1 bundler` to add Ruby and Bundler to your packages
1. Add `"gem install jekyll --version \"~> 3.9.2\""` to your init hook. This will install the Jekyll gem in your local project.
1. Start your `devbox shell`, then run `jekyll new myblog` to create the starter project.
1. From here you can install the project using Bundler, and start the server using `jekyll serve`. See the scripts in this example for more details.