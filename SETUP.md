# Portfolio Setup Instructions

## ⚠️ IMPORTANT: Image Setup

All images are currently broken because they reference local file paths. To fix this:

### Step 1: Create the Assets Folder Structure
Create the following folders in your repository:
```
assets/
├── portrait/
├── images/
│   └── social_media/
└── documents/
```

### Step 2: Add Your Images

1. **Portrait Image**: Place your portrait image at:
   ```
   assets/portrait/mahmoud-removebg-preview.png
   ```

2. **Portfolio Images**: Upload all design images to:
   ```
   assets/images/social_media/
   ```
   
   Examples:
   - `d1@lst.png`
   - `d1@computopia.png`
   - `d1@haramlek.png`
   - etc. (all 214+ images)

3. **Resume/CV**: Place your resume at:
   ```
   assets/documents/Mahmoud_Ahmed.pdf
   ```

### Step 3: Commit Changes

```bash
git add -A
git commit -m "Add portfolio images and assets"
git push
```

## File Path Reference

The JavaScript file (`mahmoud_portfolio_data.js`) already has the correct relative paths:
- `assets/portrait/mahmoud-removebg-preview.png` - Portrait
- `assets/documents/Mahmoud_Ahmed.pdf` - Resume
- `assets/images/social_media/` - All portfolio images

## Notes

- Do NOT use `file:///` local paths in web applications
- Use relative paths instead (e.g., `assets/images/...`)
- GitHub Pages and web servers cannot access local file system
- All image files must be in the repository for them to load on the live site

## Testing Locally

To test locally with Python's simple server:
```bash
python -m http.server 8000
```

Then visit: `http://localhost:8000`