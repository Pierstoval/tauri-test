# Tauri test with Svelte

This small app is a simple [Tauri](https://tauri.studio/) + [Svelte](https://svelte.dev/) (using [Svelte kit](https://kit.svelte.dev/)) setup.

## How to install

* Install **system dependencies** depending on your platform (linux, mac, windows) as stated in Tauri's docs there: https://tauri.studio/en/docs/getting-started/intro
* Install Node.js
* Install Yarn
* Clone the project
* Run `yarn install`

### Small tip: Docker

You can use the `pierstoval/rust-node` Docker image to run this project!

It contains **all** the binaries and system dependencies you need.

Just use it in a `docker-compose.yaml` file, or raw like this:

```
$ docker run -it --rm -v `pwd`:/srv --workdir=/srv pierstoval/rust-node bash
root@f081718106d1:/srv# ...
```

Then you can run all the commands in the next section, like `yarn install` and all other ones, and it should just work 😉.

Feel free to **create an issue** if anything goes wrong!

## How to build

* Run `yarn build`
* Run `yarn tauri build`
* Get your binary in `src-tauri/target/releases/` (it's named `compotes` here, because it's fun)
* Enjoy! 🚀
