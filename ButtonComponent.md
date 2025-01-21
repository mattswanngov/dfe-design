## Button Component Documentation

### Overview
The button component is a key UI element used to trigger actions. It is designed to be accessible, scalable, and flexible, allowing it to be adapted across multiple projects.

---

### Button States

Each button supports the following states:

1. **Default**: Standard button appearance, ready for interaction.
2. **Hover**: Provides visual feedback when hovered.
3. **Focused**: Highlighted when focused for accessibility.
4. **Disabled**: Grayed out and non-interactive.
5. **Outline**: A bordered version of the button.
6. **No Background (Nob)**: Minimal style with just text and icons.

---

### Button Types

The button is available in the following types to support various use cases:

- **Primary**: Main action buttons with high visibility.
- **Secondary**: For secondary actions.
- **Tertiary**: Minimal styling, lower emphasis.
- **CAL Primary/Secondary**: Custom styles tailored for specific brands.
- **Success**: Indicates successful actions.
- **Warning**: Used for cautionary actions.
- **Error**: Alerts and errors.

---

### Button Sizes

Each button type is available in various sizes:

- **XS (Extra Small)**
- **SM (Small)**
- **MD (Medium)**
- **LG (Large)**
- **XL (Extra Large)**

Each size adjusts properties like padding, font size, and overall dimensions.

---

### Design Tokens

The button component is styled using the following design tokens:

```json
{
    "button_primary_background": {
        "$value": "#004D44",
        "$type": "color"
    },
    "button_primary_text_color": {
        "$value": "#FFFFFF",
        "$type": "color"
    },
    "button_secondary_background": {
        "$value": "#00D237",
        "$type": "color"
    },
    "button_secondary_text_color": {
        "$value": "#000000",
        "$type": "color"
    },
    "button_border_radius": {
        "$value": "8px",
        "$type": "dimension"
    },
    "button_padding_horizontal": {
        "$value": "16px",
        "$type": "dimension"
    },
    "button_padding_vertical": {
        "$value": "8px",
        "$type": "dimension"
    },
    "button_font_size": {
        "$value": "16px",
        "$type": "typography"
    },
    "button_font_weight": {
        "$value": "600",
        "$type": "fontWeight"
    }
}
```

---

### Usage Guidelines

- Use **Primary** buttons for key actions such as form submissions.
- Use **Secondary** or **Tertiary** buttons for less important actions.
- Ensure **Focus** states meet accessibility requirements.
- Use appropriate **size variants** based on layout and screen space.

---

### Implementation

Example HTML structure:

```html
<button class="btn btn-primary">Click Me</button>
```

Example CSS:

```css
.btn-primary {
    background-color: var(--button-primary-background);
    color: var(--button-primary-text-color);
    padding: var(--button-padding-vertical) var(--button-padding-horizontal);
    border-radius: var(--button-border-radius);
    font-size: var(--button-font-size);
    font-weight: var(--button-font-weight);
}
```

---

### Accessibility Considerations

- Ensure focus indicators are visible and meet WCAG 2.1 AA standards.
- Provide sufficient contrast between text and background colors.
- Use ARIA attributes where necessary for better screen reader support.

---

This documentation serves as a reference for implementing and customizing the button component across various projects.

