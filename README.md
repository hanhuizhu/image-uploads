# Image Uploads

Automatically upload images to this repository and get direct raw URLs.

## Ways to upload

### 🖥️ Web Upload (GitHub Pages)

Upload images via a web interface at:

**https://hanhuizhu.github.io/image-uploads**

1. Enter your GitHub token (requires `public_repo` scope)
2. Drag & drop or select an image
3. Click upload → get a `raw.githubusercontent.com` URL instantly

> Token is stored only in your browser's localStorage and never sent anywhere except GitHub API.

### 📝 Issue Upload

1. Create a [new Issue](https://github.com/hanhuizhu/image-uploads/issues/new)
2. Paste images into the description
3. GitHub Action automatically commits them and posts the URLs

## Image URLs

All uploaded images are accessible via:

```
https://raw.githubusercontent.com/hanhuizhu/image-uploads/main/images/<path>
```

## Notes

- Supported formats: PNG, JPG, JPEG, GIF, SVG, WebP
- Files are stored in `images/` directory:
  - Web uploads → `images/upload/`
  - Issue uploads → `images/issue-<N>/`
