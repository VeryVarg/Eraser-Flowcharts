# Contributing to Eraser-Flowcharts

Thank you for contributing to this flowchart repository! This guide will help you add and maintain flowcharts effectively.

## Adding a New Flowchart

### Step 1: Create Your Flowchart

1. Go to [Eraser.io](https://eraser.io)
2. Create your flowchart using the diagram editor
3. Use clear labels and descriptions
4. Follow any relevant naming conventions

### Step 2: Export Your Flowchart

**Option A: Export as .eraserdiagram file**
- Click "Export" in Eraser.io
- Save the `.eraserdiagram` file

**Option B: Save diagram code**
- Copy the diagram code from Eraser.io
- Save it as a `.md` or `.txt` file

### Step 3: Organize in Repository

1. Choose or create an appropriate subdirectory in `flowcharts/`:
   ```bash
   flowcharts/
     └── [project-or-category-name]/
   ```

2. Add your diagram file with a descriptive name:
   ```bash
   flowcharts/my-project/user-authentication-flow.eraserdiagram
   ```

### Step 4: Export Visual Representations

1. Export your flowchart as PNG and/or SVG from Eraser.io
2. Add the exported images to the corresponding path in `exports/`:
   ```bash
   exports/my-project/user-authentication-flow.png
   exports/my-project/user-authentication-flow.svg
   ```

### Step 5: Document Your Flowchart

1. Copy the template from `templates/FLOWCHART_TEMPLATE.md`
2. Create a new document in `docs/` or alongside your flowchart
3. Fill in all relevant details:
   - Clear description
   - Purpose and context
   - Date created/updated
   - Links to source and exports

### Step 6: Update the Index (Optional)

If you have an `INDEX.md` file in `docs/`, add your new flowchart to the appropriate section.

## Best Practices

### Naming Conventions

- Use lowercase with hyphens: `user-registration-flow.eraserdiagram`
- Be descriptive: Avoid generic names like `diagram1.eraserdiagram`
- Use consistent prefixes for related diagrams

### Organization

- Group related flowcharts in the same directory
- Use subdirectories for large projects or categories
- Keep the structure shallow (2-3 levels max)

### Documentation

- Always include a description of what the flowchart represents
- Document assumptions and constraints
- Link related flowcharts together
- Keep documentation up-to-date when diagrams change

### Version Control

- Commit diagram source files (`.eraserdiagram`, `.md`)
- Commit exported images for easy reference
- Write clear commit messages describing changes
- Update "Last Updated" dates in documentation

## File Organization Example

```
├── flowcharts/
│   └── e-commerce-platform/
│       ├── checkout-process.eraserdiagram
│       ├── payment-gateway.eraserdiagram
│       └── inventory-management.eraserdiagram
├── exports/
│   └── e-commerce-platform/
│       ├── checkout-process.png
│       ├── checkout-process.svg
│       ├── payment-gateway.png
│       └── inventory-management.png
└── docs/
    └── e-commerce-platform/
        ├── checkout-process.md
        ├── payment-gateway.md
        └── inventory-management.md
```

## Questions?

If you have questions about contributing, please open an issue or refer to the main [README.md](README.md).
