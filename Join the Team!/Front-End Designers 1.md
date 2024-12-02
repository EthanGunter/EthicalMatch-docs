# EthicalMatch UI/UX Designer Onboarding
As a UI/UX designer, your work is crucial in shaping the visual and interactive elements of our platform. This guide will help you contribute effectively within our design-first, collaborative workflow.

---

## Recommended Tools for Collaborative Design
While you are free to use the tools you're most comfortable with, the following are commonly used in our community for their collaborative features:
- **Figma**: Great for collaborative wireframing and prototyping.
- **Adobe XD**: A robust tool for creating interactive designs.
- **Sketch**: Popular for high-fidelity mockups.
- **Excalidraw**: Simple and open-source for quick sketches.

For embedding finalized designs in our documentation repository, export images in **SVG** or **PNG** format.

---

## Design Expectations
To ensure your designs are as useful as possible to frontend developers, please adhere to the following guidelines:

### 1. **Clarity And Consistency**
- Use consistent layouts and design patterns.
- Label interactive elements clearly (e.g., buttons, dropdowns).
- Reference our [Design Style Guide](Documentation%20Guidelines.md#style-guide) for visual standards.

### 2. **Accessibility**
- Consider color contrast, font sizes, and keyboard navigation in your designs.
- Include annotations for accessibility features, such as ARIA roles or tab orders.

### 3. **Detailing Interactions**
- Use annotations to describe how components behave under various conditions (e.g., hover states, errors).
- If creating a prototype, include key transitions and animations.

### 4. **File Organization**
- Save exported images in the `designs` folder within the relevant repository.
  - Example: `src/assets/designs/FeatureName-Wireframe.png`
- Embed images directly in markdown documents using this syntax:
  ```markdown
  ![Alt text for accessibility](relative/path/to/image.png)