# Northskill Mechanic

The website for the mechanic shop. Built with Hugo. 

## Prerequisites

- **Hugo Extended** (v0.120.0 or later) — [Installation guide](https://gohugo.io/installation/)
- **Go** (v1.21 or later) — Required for Hugo Modules — [Installation guide](https://go.dev/doc/install)

No Node.js or npm required — CSS is pre-compiled.


## Block-Based Page Layout

Pages are composed from reusable "blocks" defined in front matter. The theme loops through the `blocks` array and renders each block partial.

### How It Works

1. Define blocks in your page's front matter under the `blocks` key
2. Each block must have a `block` field matching a partial name in `layouts/partials/blocks/`
3. Blocks render in the order they appear in the array
4. Additional parameters are passed to the block partial



### Production Build

```bash
hugo --minify
```

Output goes to `public/` directory.

