# sbox-annotations

A set of [external annotations](https://www.jetbrains.com/help/rider/Code_Analysis__External_Annotations.html) for [s&box](https://sbox.game/) that can be used to provide some hints to [Rider](https://www.jetbrains.com/rider/)'s code analysis.

There are only a small handful of annotations, but it's enough to fix the most frequent "unused class/property" warnings.

## How to use

You'll probably want to enable `Nullables` in your s&box project settings and restart the editor to regenerate the project files. The `*.xml` files need to be in an `ExternalAnnotations/` folder next to the root `.sbproj` file in your project. You can either:

- Manually copy the files into your project
- Add this repo as a submodule to your project's git repo

Restart Rider and you're good to go.

## Adding annotations

The documentation on how external annotations work is linked at the top of this readme. Finding the ID for a member to annotate can be done by navigating to its declaration, right-clicking on it, and selecting `Copy / Paste Special` > `Copy Code Reference...` > `XML-Doc ID`
