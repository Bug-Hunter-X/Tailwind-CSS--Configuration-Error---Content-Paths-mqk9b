# Tailwind CSS Configuration Error: Content Paths

This repository demonstrates a common configuration error in Tailwind CSS where the `content` option in `tailwind.config.js` is incorrectly specified, preventing Tailwind from processing your HTML and JavaScript files.

## Problem

Tailwind CSS might not apply custom styles or classes you've added because the paths in the `content` array are incorrect or point to the wrong directory.  This commonly leads to the error that your custom classes are not defined, despite being properly implemented.

## Solution

The solution involves correctly configuring the `content` option in your `tailwind.config.js` file to point to the directories containing your HTML and JavaScript files where Tailwind's directives are used.

Check that the path is accurate relative to the location of your `tailwind.config.js` file.  Common mistakes involve typos or using an absolute path when a relative one is needed.

## How to Reproduce

1. Clone this repository.
2. Notice the incorrect `content` path in `tailwind.config.js`.
3. Run your build process or Tailwind JIT compilation.  You'll see that the custom styles are not applied.
4. Switch to `tailwind.config.fixed.js` to see the corrected configuration and the correct application of styles.

## Related Resources

* [Tailwind CSS Documentation on Configuration](https://tailwindcss.com/docs/configuration)
* [Tailwind CSS Documentation on Content](https://tailwindcss.com/docs/content-configuration)