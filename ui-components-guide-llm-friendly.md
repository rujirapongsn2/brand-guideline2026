# Softnix UI Components Guide (LLM-Friendly)

This document maps the HTML/CSS implementation of Softnix's UI components to the Brand Guidelines. use this as a reference when generating or analyzing UI code.

## 1. Design Tokens

### Colors (`:root` variables)
| Variable | Value/Hex | Description |
| :--- | :--- | :--- |
| **Primary** | | |
| `--orange` | `#F3903F` | Softnix Orange (Core Brand) |
| `--orange-light` | `#F9B77A` | Lighter Orange for dark mode text/accents |
| `--yellow` | `#FDC70C` | Softnix Yellow |
| `--lime` | `#A9CB2E` | Softnix Lime |
| `--lime-light` | `#C4DD6B` | Lighter Lime for dark mode text/accents |
| `--blue` | `#2786C2` | Softnix Blue |
| `--blue-light` | `#5EADD6` | Lighter Blue for dark mode text/accents |
| **Neutrals** | | |
| `--dark-navy` | `#0D1B2A` | Product Background (Dark Mode) |
| `--charcoal` | `#1B263B` | Surface Color (Dark Mode) |
| `--slate` | `#778DA9` | Secondary Text / Borders |
| `--light-slate` | `#9BA8B4` | Muted Text (Dark Mode) |
| `--off-white` | `#F8F9FA` | Page Background (Light Mode) |
| `--pure-white` | `#FFFFFF` | Surface Color (Light Mode) |
| **Semantic** | | |
| `--success` | `#A9CB2E` | Lime Green |
| `--warning` | `#FDC70C` | Yellow |
| `--error` | `#E53935` | Red |
| `--info` | `#2786C2` | Blue |

### Product Layers & Gradients
Components adapt their "Theme Color" based on the product layer.

| Layer | Product Families | Theme Color/Gradient | Variable |
| :--- | :--- | :--- | :--- |
| **Layer 3** | AI-Ready Agents, DFlow | **Yellow-Lime Gradient**<br>(`#FDC70C` → `#A9CB2E`) | `--gradient-l3` |
| **Layer 2** | Softnix GenAI, Logger | **Orange Gradient**<br>(`#F3903F` → `#D67020`) | `--gradient-l2` |
| **Layer 1** | Data Platform, LLM | **Blue Gradient**<br>(`#2786C2` → `#1A5A8A`) | `--gradient-l1` |

---

## 2. Component Specifications

### 2.1 Form Elements
**Input, Checkbox, Radio, Toggle**

#### Inputs
- **Base Style**: Rounded corners (`8px`), `1rem` padding.
- **Light Mode**: White bg, `#e0e0e0` border.
- **Dark Mode**: Dark Navy bg, `rgba(255,255,255,0.2)` border.
- **Focus State**: Border becomes **Theme Color**. Box-shadow adds a 3px glow of the Theme Color (at ~15-25% opacity).

```html
<!-- Example: Layer 3 (Lime) Input Focus -->
<input style="border-color: var(--lime); box-shadow: 0 0 0 3px rgba(169,203,46,0.15);">
```

#### Checkbox & Radio
- **Checked State**: Background becomes **Theme Gradient** (e.g., `--gradient-l3` for Layer 3).
- **Unchecked**: Gray border.

#### Toggle Switch
- **ON State**: Track background becomes **Theme Gradient**.
- **OFF State**: Gray track (`#d0d0d0`).

---

### 2.2 Feedback & Status
**Alerts, Tooltips, Spinners**

#### Alerts (Toast)
- **Background**: Low opacity version of the semantic or theme color (e.g., `rgba(169,203,46,0.15)` for Layer 3).
- **Text**: Brand color (e.g., `#7FA31E`).
- **Dark Mode**: Often adds a thin border `1px solid rgba(..., 0.3)`.

#### Tooltips
- **Background**: Solid **Theme Color** (e.g., `--lime`) or **Theme Gradient**.
- **Text**: Contrast color (Dark Navy for Lime/Yellow, White for Orange/Blue).
- **Arrow**: Matches background color.

#### Spinners
- **Style**: Circular border with transparent top.
- **Color**: Border is low opacity theme color; Top border is solid **Theme Color**.

---

### 2.3 Navigation
**Tabs, Pagination, Breadcrumbs**

#### Tabs & Pagination
- **Active State**: Background is **Theme Color** (solid) or **Theme Gradient**. Text matches contrast rules.
- **Inactive**: Neutral background (`#e8e8e8` light / `rgba(255,255,255,0.1)` dark).

#### Breadcrumbs
- **Links**: colored with **Theme Color** (e.g., `#F3903F` for Layer 2).
- **Separators**: Slate gray.

---

### 2.4 Interactive Components
**Avatars, Chips, Badges**

#### Avatars
- **Background**: Solid **Theme Color**.
- **Text**: Contrast color.
- **Status Indicator**: Positioned bottom-right.

#### Chips (Tags)
- **Style**: Rounded pill shape (`20px` radius).
- **Background**: Low opacity theme color.
- **Gradient Variant**: Text can use `background-clip: text` with the **Theme Gradient**. Border can be solid theme color.

#### Badges (Notification)
- **Background**: Solid **Theme Color** or **Theme Gradient**.
- **Text**: Small, bold, contrast color.
- **Position**: Top-right of icon/container.

---

## 3. Implementation Rules for LLMs

1.  **Identify the Layer**: First determine if the UI belongs to Layer 1 (Blue), Layer 2 (Orange), or Layer 3 (Yellow-Lime).
2.  **Apply CSS Variables**: Use the specific variables (`--gradient-l3`, `--lime`, etc.) rather than hardcoded hex values where possible, but if inline styles are required, use the Hex codes mapped in the Design Tokens table.
3.  **Gradients vs Solids**:
    -   Use **Gradients** for: Primary buttons, Toggle switches (ON), Checkboxes (Checked), Mode badges, decorative headers.
    -   Use **Solids** for: Text links, Borders, Avatars (bg), Notification Badges (bg).
4.  **Dark Mode Adaptation**:
    -   Backgrounds shift to `var(--dark-navy)` or `var(--charcoal)`.
    -   Borders become translucent white (`rgba(255,255,255,0.1)`).
    -   Text colors shift to "Light" variants (`--lime-light`, `--orange-light`) for better contrast against dark backgrounds.
