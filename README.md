# Image Uploads

Automatically upload images pasted in Issues to this repository via GitHub Actions.

## How it works

1. Create a new Issue and paste images into the description
2. The GitHub Action workflow triggers on `issues: opened`
3. It extracts image URLs from the Issue body and downloads them
4. Images are committed to `images/issue-<N>/`
5. A comment is posted to the Issue with direct raw image URLs

## How to use

1. Go to the [Issues](https://github.com/hanhuizhu/image-uploads/issues) tab
2. Click "New Issue"
3. Paste or drag-drop images into the description
4. Submit the issue
5. Wait a few seconds for the Action to complete
6. Check the issue comment for uploaded image URLs

## Access uploaded images

Uploaded images are accessible via:

```
https://raw.githubusercontent.com/hanhuizhu/image-uploads/main/images/issue-<N>/<filename>
```

## Notes

- Only public Issues will trigger the workflow
- Supported formats: PNG, JPG, JPEG, GIF, SVG, WebP
- GitHub Issue attachment URLs are also supported
