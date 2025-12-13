# Softnix Slide Usage Guidelines 2026 (LLM-Friendly)

## 📋 Overview
This document provides comprehensive guidelines for creating Softnix-branded presentation slides. It's optimized for LLM understanding with clear structure, semantic organization, and detailed specifications.

## 🎨 Color Palette

### Primary Brand Colors
```markdown
- Softnix Orange: #F3903F (RGB: 243, 144, 63) - Energy, Innovation
- Softnix Yellow: #FDC70C (RGB: 253, 199, 12) - Brightness, Insight
- Softnix Lime: #A9CB2E (RGB: 169, 203, 46) - Growth, AI Ready
- Softnix Blue: #2786C2 (RGB: 39, 134, 194) - Trust, Enterprise
```

### Neutral Colors
```markdown
- Dark Navy: #0D1B2A - Professional backgrounds
- Charcoal: #1B263B - Secondary backgrounds
- Light Slate: #778DA9 - Secondary text, borders
- Off White: #F8F9FA - Page backgrounds
- Pure White: #FFFFFF - Text on dark backgrounds
```

### Brand Gradients
```markdown
- Sunrise: linear-gradient(135deg, #F3903F 0%, #FDC70C 100%)
- Nature: linear-gradient(135deg, #A9CB2E 0%, #2786C2 100%)
- Full Spectrum: linear-gradient(135deg, #F3903F 0%, #FDC70C 33%, #A9CB2E 66%, #2786C2 100%)
- Dark Mode: linear-gradient(180deg, #0D1B2A 0%, #1B263B 100%)
```

## 🖼️ Slide Backgrounds

### Dark Theme Backgrounds
1. **Dark Theme Standard**: Dark Navy Gradient (#0D1B2A to #1B263B)
   - Usage: Professional presentations, formal settings
   - File: `images/slide_bg_dark.png`

2. **Dark Theme Side Color**: Dark Navy with Side Accent
   - Usage: Modern presentations, visual interest
   - File: `images/slide_bg_dark_sidecolor.png`

### Light Theme Backgrounds
1. **Light Theme Standard**: Clean White/Grey Gradient
   - Usage: Daytime presentations, bright environments
   - File: `images/slide_bg_light.png`

2. **Light Theme Side Color**: Light with Side Accent
   - Usage: Friendly presentations, collaborative settings
   - File: `images/slide_bg_light_sidecolor.png`

## 🎯 Gradient Background Options (Dark Theme)

### Option 1: Subtle Gradient
```css
linear-gradient(135deg, #0D1B2A 0%, #1B263B 50%, #0F2238 100%)
```
- **Usage**: Content slides for readability
- **Characteristics**: Smooth transition, low contrast

### Option 2: Bold Gradient with Accent
```css
linear-gradient(135deg, #0D1B2A 0%, #1B263B 50%, #0F3A52 100%) + Radial Glow
```
- **Usage**: Title slides, section dividers
- **Characteristics**: Deeper colors with glow effect

### Option 3: Vibrant Gradient
```css
linear-gradient(135deg, #0D1B2A, #1B263B, #0F3A52) + Orange Glow
```
- **Usage**: Highlight slides, emphasis points
- **Characteristics**: Orange glow for visual impact

## 📐 Slide Layouts

### Dark Theme Slides

#### 1. Title Slide
```markdown
- Background: Dark Navy (#0D1B2A)
- Logo: Softnix White (centered, 45px height)
- Title: Poppins 700, 44-60pt, White
- Subtitle: Sarabun 400, 24-28pt, Light Slate (#778DA9)
- Accent: Radial gradient glow (top-right)
```

#### 2. Section Divider
```markdown
- Background: Dark Navy (#0D1B2A)
- Left Border: 6px gradient (Orange → Yellow → Lime → Blue)
- Section Number: Poppins 600, 14pt, Orange (#F3903F)
- Section Title: Poppins 700, 36-44pt, White
```

#### 3. Content Slide
```markdown
- Background: Dark Navy (#0D1B2A)
- Title: Poppins 600, 28-32pt, White
- Bullet Points: Sarabun 400, 18-22pt, Off-White
- Bullet Icons: 6px circles in brand colors
- Spacing: 15px between elements
```

#### 4. Two Column Layout
```markdown
- Background: Dark Navy (#0D1B2A)
- Title: Poppins 600, 28-32pt, White
- Columns: 50/50 split with 15px gap
- Left Column: Orange accent (#F3903F, 15% opacity)
- Right Column: Blue accent (#2786C2, 15% opacity)
```

#### 5. Image Focus Slide
```markdown
- Background: Dark Navy (#0D1B2A)
- Layout: 40/60 split (text/image)
- Image Area: Gradient overlay (Yellow → Lime, 30% opacity)
- Text: Poppins 600, 24-28pt, White
```

#### 6. Quote Slide
```markdown
- Background: Dark Navy (#0D1B2A)
- Quote Mark: 2rem, Orange (#F3903F)
- Quote Text: Poppins 500, 24-28pt, White, Italic
- Attribution: Sarabun 400, 16-18pt, Light Slate (#778DA9)
```

#### 7. Data/Chart Slide
```markdown
- Background: Dark Navy (#0D1B2A)
- Title: Poppins 600, 28-32pt, White
- Chart Colors: Brand colors in sequence (Orange, Yellow, Lime, Blue)
- Data Bars: 60-80% height, rounded corners
```

#### 8. Thank You Slide
```markdown
- Background: Dark Navy Gradient (#0D1B2A → #1B263B)
- Title: "Thank You" in Full Spectrum Gradient
- Subtitle: Sarabun 400, 16-18pt, Light Slate (#778DA9)
- Accent: Radial gradient glow (bottom-left)
```

### Light Theme Slides

#### 1. Title Slide (Light)
```markdown
- Background: Off White (#F8F9FA)
- Logo: Softnix Standard (centered, 45px height)
- Title: Poppins 700, 44-60pt, Dark Navy (#0D1B2A)
- Subtitle: Sarabun 400, 24-28pt, Light Slate (#778DA9)
- Accent: Radial gradient glow (top-right, 10% opacity)
```

#### 2. Content Slide (Light)
```markdown
- Background: Off White (#F8F9FA)
- Title: Poppins 600, 28-32pt, Dark Navy (#0D1B2A)
- Bullet Points: Sarabun 400, 18-22pt, Slate (#415A77)
- Bullet Icons: 6px circles in brand colors
- Spacing: 15px between elements
```

#### 3. Two Column Layout (Light)
```markdown
- Background: Off White (#F8F9FA)
- Title: Poppins 600, 28-32pt, Dark Navy (#0D1B2A)
- Columns: 50/50 split with 15px gap
- Cards: White background with colored borders
- Left Border: 3px Orange (#F3903F)
- Right Border: 3px Blue (#2786C2)
```

## 📝 Typography Guidelines

### Font Families
```markdown
- Headings: Poppins (Geometric Sans-serif)
- Body Text: Sarabun (Thai Sans-serif)
```

### Type Scale (PowerPoint Points)
```markdown
- Main Title: Poppins 700, 44-60pt
- Section Title: Poppins 600, 36-44pt
- Subtitle: Poppins 500, 24-28pt
- Body Text: Sarabun 400, 18-22pt
- Caption/Label: Sarabun 400, 14-16pt
```

### Font Weights
```markdown
- Display/Headings: Poppins 700 (Bold)
- Section Titles: Poppins 600 (SemiBold)
- Subtitles: Poppins 500 (Medium)
- Body Text: Sarabun 400 (Regular)
- Captions: Sarabun 400 (Regular)
```

## 📊 Chart Colors

### Recommended Color Sequence
```markdown
1. Orange: #F3903F (Primary data)
2. Blue: #2786C2 (Secondary data)
3. Lime: #A9CB2E (Tertiary data)
4. Yellow: #FDC70C (Quaternary data)
5. Light Slate: #778DA9 (Quinary data)
6. Charcoal: #1B263B (Senary data)
```

### Pie Chart Recommendations
```markdown
- For >4 segments: Use opacity variations (100%, 80%, 60%, 40%)
- Maintain color consistency with brand palette
- Ensure sufficient contrast between segments
```

## ✅ Do's & Don'ts

### ✅ Do's (Best Practices)
```markdown
1. Use readable font sizes (≥18pt for body text)
2. Maintain adequate white space
3. Use bullet points instead of long paragraphs
4. Use high-quality images (sufficient resolution)
5. Maintain consistent layout throughout deck
6. Use accent colors to highlight key points
7. Keep logo in consistent position
8. Ensure good contrast between text and background
```

### ❌ Don'ts (Avoid These)
```markdown
1. Overcrowd slides with too much text
2. Use more than 2 font families
3. Use excessive animations
4. Use pixelated or low-resolution images
5. Use non-brand colors
6. Use busy or patterned backgrounds
7. Use light text on light backgrounds
8. Use unprofessional clipart or stock images
```

## 💡 Pro Tips

### Rule of 6
```markdown
- No more than 6 bullet points per slide
- No more than 6 words per bullet point
```

### One Idea per Slide
```markdown
- Each slide should have only one main message
- Use multiple slides for complex concepts
```

### Visual Hierarchy
```markdown
- Use font size and weight to indicate importance
- Larger = More important, Smaller = Supporting
```

### Aspect Ratio
```markdown
- Standard: 16:9 (1920×1080 pixels)
- Compatible with modern widescreen displays
```

### Export Quality
```markdown
- Export as high-quality PDF or PPTX
- Ensure images maintain resolution
- Test on target display devices
```

## 🎨 Design Tips for Different Slide Types

### Title Slides
```markdown
- Use gradient backgrounds for visual interest
- Keep text minimal (title + subtitle only)
- Include logo prominently
- Use glow effects sparingly
```

### Content Slides
```markdown
- Use subtle gradients for readability
- Limit to 3-5 bullet points maximum
- Use icons to enhance visual appeal
- Maintain consistent spacing
```

### Data/Chart Slides
```markdown
- Use brand colors consistently
- Label axes clearly
- Highlight key data points
- Keep legends simple and readable
```

### Quote Slides
```markdown
- Use large quote marks for visual impact
- Keep attribution clear but subtle
- Use italics for quote text
- Center-align text for balance
```

## 🔧 Technical Specifications

### Slide Dimensions
```markdown
- Standard: 1920×1080 pixels (16:9 aspect ratio)
- Safe Margins: 60px from all edges
- Content Area: 1800×960 pixels
```

### Color Accessibility
```markdown
- Minimum contrast ratio: 4.5:1 for normal text
- Minimum contrast ratio: 3:1 for large text
- Test colors with accessibility tools
```

### File Formats
```markdown
- Source: PowerPoint (.pptx) or Keynote (.key)
- Export: PDF (high quality) for distribution
- Images: PNG (transparent) or JPG (photographic)
```

## 📁 File Organization

### Recommended Structure
```markdown
project/
├── slides/
│   ├── templates/
│   │   ├── dark-theme.pptx
│   │   ├── light-theme.pptx
│   │   └── gradient-options.pptx
│   ├── assets/
│   │   ├── images/
│   │   ├── icons/
│   │   └── logos/
│   └── final/
│       └── presentation-final.pptx
└── README.md
```

## 🎯 Brand Consistency Checklist

```markdown
[ ] Use correct brand colors
[ ] Use approved fonts (Poppins + Sarabun)
[ ] Maintain proper logo usage
[ ] Follow typography guidelines
[ ] Use brand-approved gradients
[ ] Maintain consistent spacing
[ ] Use proper contrast ratios
[ ] Follow slide layout templates
[ ] Include required legal disclaimers
[ ] Export in correct format
```

This comprehensive guide ensures all Softnix presentations maintain brand consistency while being optimized for readability and professional impact.