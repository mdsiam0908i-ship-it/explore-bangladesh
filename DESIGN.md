---
name: Explore Bangladesh
colors:
  surface: '#f9f9fc'
  surface-dim: '#dadadc'
  surface-bright: '#f9f9fc'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f3f6'
  surface-container: '#eeeef0'
  surface-container-high: '#e8e8ea'
  surface-container-highest: '#e2e2e5'
  on-surface: '#1a1c1e'
  on-surface-variant: '#3f4944'
  inverse-surface: '#2f3133'
  inverse-on-surface: '#f0f0f3'
  outline: '#6f7a73'
  outline-variant: '#bec9c2'
  surface-tint: '#046c50'
  primary: '#00503a'
  on-primary: '#ffffff'
  primary-container: '#006a4e'
  on-primary-container: '#92e7c3'
  inverse-primary: '#83d7b4'
  secondary: '#7a5900'
  on-secondary: '#ffffff'
  secondary-container: '#fec64b'
  on-secondary-container: '#725300'
  tertiary: '#90000a'
  on-tertiary: '#ffffff'
  tertiary-container: '#bd0011'
  on-tertiary-container: '#ffc9c3'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#9ef4d0'
  primary-fixed-dim: '#83d7b4'
  on-primary-fixed: '#002116'
  on-primary-fixed-variant: '#00513b'
  secondary-fixed: '#ffdea2'
  secondary-fixed-dim: '#f5be43'
  on-secondary-fixed: '#261900'
  on-secondary-fixed-variant: '#5c4200'
  tertiary-fixed: '#ffdad6'
  tertiary-fixed-dim: '#ffb4ab'
  on-tertiary-fixed: '#410002'
  on-tertiary-fixed-variant: '#93000a'
  background: '#f9f9fc'
  on-background: '#1a1c1e'
  surface-variant: '#e2e2e5'
typography:
  headline-xl:
    fontFamily: Plus Jakarta Sans
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-xl-mobile:
    fontFamily: Plus Jakarta Sans
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: Be Vietnam Pro
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Be Vietnam Pro
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-md:
    fontFamily: Be Vietnam Pro
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
    letterSpacing: 0.01em
  label-sm:
    fontFamily: Be Vietnam Pro
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  gutter: 16px
  margin-mobile: 16px
  margin-desktop: 64px
---

## Brand & Style
The design system for Explore Bangladesh is built to evoke a sense of discovery, reliability, and warmth. The target audience includes both international tourists seeking cultural immersion and local travelers looking for hidden gems. 

The visual style is **Corporate / Modern** with a strong leaning towards **Minimalism**. This ensures that the vibrant photography of Bangladesh’s landscapes remains the focal point. The interface uses generous whitespace to reduce cognitive load, paired with high-quality typography to establish authority and trust. The emotional response should be one of optimistic curiosity—a feeling that the journey ahead is well-planned and welcoming.

## Colors
The color palette for the design system is inspired by the natural landscape and heritage of the region.

- **Primary (#006A4E):** A deep, lush green representing the Delta's fertility and the national identity. Used for primary actions and brand presence.
- **Secondary (#F4BD42):** A warm, sun-drenched amber used for highlights, ratings, and call-outs to evoke the golden hour.
- **Tertiary (#E3101B):** A vibrant crimson used sparingly for critical alerts or specific cultural heritage markers.
- **Neutral (#1A1C1E):** A deep charcoal for typography to maintain high legibility and a professional groundedness.

The default color mode is **light**, utilizing soft off-white backgrounds (#FDFDFD) to keep the experience feeling airy and accessible.

## Typography
The typography strategy prioritizes approachability and clarity. 

**Plus Jakarta Sans** is used for all headlines. Its soft, rounded terminals provide a welcoming and optimistic feel that aligns with travel and exploration. **Be Vietnam Pro** is utilized for body copy and labels; its contemporary and clean construction ensures high readability during long-form reading, such as itinerary descriptions or travel guides.

For mobile devices, `headline-xl` scales down to 32px to ensure titles remain within the viewport and maintain a proper visual hierarchy without overwhelming the user.

## Layout & Spacing
The design system employs a **12-column fluid grid** for desktop environments and a **4-column fluid grid** for mobile. 

The spacing rhythm is built on a strict **8px baseline**. 
- **Margins:** 16px on mobile to maximize screen real estate, increasing to 64px on desktop to provide a premium, airy feel.
- **Gutters:** Fixed at 16px to maintain consistent breathing room between content modules.
- **Vertical Spacing:** Content blocks are separated by `xl` (40px) units, while related elements within a block use `md` (16px) or `sm` (8px) units to create a clear logical grouping.

## Elevation & Depth
In this design system, depth is communicated through **Ambient Shadows** and **Tonal Layers**. 

Physicality is subtle:
1.  **Level 0 (Surface):** The base background layer, flat and neutral.
2.  **Level 1 (Cards):** Uses a very soft, diffused shadow (0px 4px 20px rgba(0, 0, 0, 0.05)) to suggest a slight lift.
3.  **Level 2 (Modals/Dropdowns):** Uses a more pronounced shadow with a slight color tint from the primary green (0px 12px 32px rgba(0, 106, 78, 0.12)) to indicate a higher position in the stack.

Avoid heavy borders; instead, use 1px strokes in a light neutral grey to define boundaries only when tonal separation is insufficient.

## Shapes
The shape language is consistently **Rounded**. A 0.5rem (8px) base radius is applied to standard UI elements like buttons and input fields. 

- **Containers & Cards:** Use `rounded-lg` (1rem / 16px) to create a friendly, modern container for imagery.
- **Large Sections:** Background containers or hero sections may use `rounded-xl` (1.5rem / 24px) for a more pronounced, "app-like" feel.
- **Icons:** Should follow a similar rounded aesthetic, avoiding sharp corners or harsh geometric ends.

## Components
- **Buttons:** Primary buttons feature a solid primary green fill with white text. Hover states should slightly darken the green. Use `rounded-md` (8px) corner radii.
- **Cards:** The hallmark of the "Explore Bangladesh" experience. They should feature a large image at the top with a `rounded-lg` (16px) clipping mask, followed by a headline and a secondary-colored rating chip.
- **Chips:** Used for "Tags" (e.g., "Nature," "Historic"). Use a light tint of the primary color with a darker green text for high contrast and accessibility.
- **Input Fields:** Use a subtle 1px border (#E0E0E0). On focus, the border transitions to the primary green with a soft outer glow.
- **Lists:** Use plenty of vertical padding (16px) between list items to maintain the minimalist aesthetic.
- **Additional Components:**
    - **Itinerary Timeline:** A vertical line component using the primary green to guide users through travel schedules.
    - **Location Badges:** Small, pill-shaped indicators for geography-specific metadata.