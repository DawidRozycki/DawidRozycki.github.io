# Jekyll SCSS File Handling Instructions

## Important: Jekyll SCSS Front Matter

When working with Jekyll SCSS files (like `assets/css/style.scss`), follow these critical rules:

### Correct SCSS Front Matter Format
Jekyll SCSS files MUST have proper YAML front matter:

```scss
---
# Only the main Sass file needs front matter (the dashes are enough)
---

@import "minima";
// Rest of your SCSS code...
```

### Key Points:
1. **Front matter is required**: Jekyll needs the `---` delimiters to process SCSS files
2. **Separate lines**: Each `---` must be on its own line
3. **No inline content**: Never write `--- --- @import` on one line
4. **Blank line after**: Add a blank line after the closing `---` before SCSS content

### Common Issues:
- **Malformed front matter** like `--- --- @import "minima";` will cause "{ expected" errors
- **Missing front matter** means Jekyll won't process the SCSS file
- **Autofix conflicts**: IDE autofix may revert changes - recreate the entire file if needed

### Diagnostic Tool Behavior:
- The `getDiagnostics` tool will show errors for Jekyll SCSS files because it treats them as pure SCSS
- This is expected behavior - Jekyll processes the front matter at build time
- Ignore SCSS diagnostics for files with Jekyll front matter

### If Front Matter Gets Corrupted:
1. Use `fsWrite` to recreate the entire file with correct format
2. Don't rely on `strReplace` for front matter fixes if autofix is interfering
3. The file will compile correctly in Jekyll even if diagnostics show errors

### File Structure:
```
assets/
  css/
    style.scss  ← Main SCSS file with front matter
```

This file should be synced to version control as it contains important styling for the Jekyll site.