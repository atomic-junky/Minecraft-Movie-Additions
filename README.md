
# Minecraft Movie Datapack

This repository contains a datapack and a resource pack that add custom items and crafting recipes from the Minecraft Movie (Addons). Textures and models from that project are reused or adapted for Minecraft Java.

## Installation

- Clone the project or download it as a zip and move the folder into your world's `datapacks` folder and `.minecraft/resourcepacks` folder.
- If you modify assets or want to rebuild, run the project's build command in PowerShell:

```shell
# Just once
beet link <world_folder_name>
```

```shell
beet build
```

or

```shell
beet watch
```

## Quick usage

- Recipes are located under `data/movie/recipe/`.
- The `assets/minecraft/items/` folder contains model overrides that map `minecraft:custom_model_data` values to `movie:item/*` models.
- Custom models and textures for the datapack are under `assets/movie/`.

## Assets & copyright

- Origin: this project is inspired by content from "Minecraft Movie Addons" (Bedrock Edition). Make sure you have permission to reuse any third-party assets before distributing the pack.
- Placeholders: many `assets/movie/textures/item/*.png` files are placeholders — replace them with the final PNGs you want to ship.

## Contributing

- To add a new item: create a recipe under `data/movie/recipe/`, add a model under `assets/movie/models/item/`, add a texture under `assets/movie/textures/item/`, and create an override in `assets/minecraft/items/` named after the recipe's result id (for example `minecraft:sheaf_pottery_sherd` → `sheaf_pottery_sherd.json`).
- Test changes by running `beet build` and loading the datapack into a world.

## License

This project is licensed under the terms of the MIT license.
See `LICENSE.md` for repository license details.
