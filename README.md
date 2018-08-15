# vue-cli-plugin-tailwind

[Tailwind CSS](https://tailwindcss.com) + [purgecss](https://www.purgecss.com) + [postcss-import](https://github.com/postcss/postcss-import)

## Install

```bash
vue add @ky-is/tailwind
```

Requires node 6 or later. 

## Usage

You can use global Tailwind classes as normal, but `shadowLookup` is also supported for `@apply` mixins directly in `.vue` modules.

In `src/components/HelloWorld.vue` of the auto-generated cli app:
```html
<style lang="postcss" scoped>
.hello {
  @apply text-purple flex;
}
</style>
```

Applies a purple text color with scoped, browser-prefixed CSS, while PurgeCSS strips all other unused colors (and classes) from the Tailwind defaults, ensuring a minimal CSS footprint.

## Thanks

https://github.com/primos63/vue-cli-plugin-tailwindcss
https://github.com/ti-pa-to/vue-cli-plugin-tailwind-purge-css
