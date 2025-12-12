# Responsive Design Visual Reference

## Viewport Width Ranges

```
┌─────────────────────────────────────────────────────────────────────┐
│                                                                         │
│   MOBILE          TABLET             DESKTOP              LARGE      │
│   320-480px       768-1023px         1024-1199px          1200px+    │
│                                                                         │
│   ┌──────┐    ┌────────────┐    ┌───────────────────┐  ┌──────────┐ │
│   │      │    │            │    │                   │  │          │ │
│   │PHONE │    │IPAD/TABLET │    │LAPTOP/DESKTOP     │  │ LARGE    │ │
│   │      │    │            │    │                   │  │ MONITOR  │ │
│   └──────┘    └────────────┘    └───────────────────┘  └──────────┘ │
│                                                                         │
└─────────────────────────────────────────────────────────────────────┘
```

---

## Navigation Scaling Example

```
Desktop (1200px+)
┌─────────────────────────────────────────────────────────────┐
│  🍲 HAPAG-ASA  |  HOME  PROGRAMS  ABOUT  👤                 │
│  font: 1.8rem  |  1.3rem
└─────────────────────────────────────────────────────────────┘

Tablet (768px)
┌──────────────────────────────────────┐
│ 🍲 HAPAG-ASA | HOME PROGRAMS ABOUT 👤│
│ font: 1.4rem | 0.95rem
└──────────────────────────────────────┘

Mobile (480px)
┌──────────────────┐
│ 🍲 HAPAG | HOME 👤│
│ 1.1rem  | 0.8rem│
└──────────────────┘
```

---

## Grid Layout Transformation

### Home Page Dashboard

```
Desktop (1200px+)
┌────────────────────────────────────────────┐
│  Announcements (3fr)     │  Updates (1fr)  │
│                          │                 │
│                          │                 │
└────────────────────────────────────────────┘

Tablet (768px)
┌─────────────────────────────┐
│  Announcements              │
│                             │
├─────────────────────────────┤
│  Updates                    │
│                             │
└─────────────────────────────┘

Mobile (480px)
┌──────────────────┐
│ Announcements    │
│                  │
├──────────────────┤
│ Updates          │
│                  │
└──────────────────┘
```

---

## Form Layout Transformation

### Profile Form

```
Desktop (1200px+)
┌─────────────────────────────────────────┐
│  First Name  │  Last Name               │
├──────────────┼──────────────────────────┤
│  Email       │  Phone                   │
└─────────────────────────────────────────┘

Tablet (768px)
┌────────────────────────────────┐
│  First Name                    │
├────────────────────────────────┤
│  Last Name                     │
├────────────────────────────────┤
│  Email                         │
├────────────────────────────────┤
│  Phone                         │
└────────────────────────────────┘

Mobile (480px)
┌──────────────┐
│ First Name   │
├──────────────┤
│ Last Name    │
├──────────────┤
│ Email        │
├──────────────┤
│ Phone        │
└──────────────┘
```

---

## Donation Form Grid

```
Desktop (1200px+)
Amount Selection:
┌──────────────┬──────────────┬──────────────┐
│   ₱500       │   ₱2,500     │   ₱5,000     │
└──────────────┴──────────────┴──────────────┘

Payment Methods:
┌──────────────┬──────────────┐
│   GCash      │   PayMaya    │
├──────────────┼──────────────┤
│   Bank       │   Credit     │
└──────────────┴──────────────┘

Tablet (768px)
Amount: ┌─────────┬─────────┐
        │ ₱500    │ ₱2,500  │
        ├─────────┴─────────┤
        │    ₱5,000         │
        └───────────────────┘

Payment: ┌─────────┐
         │ GCash   │
         ├─────────┤
         │ PayMaya │
         ├─────────┤
         │ Bank    │
         ├─────────┤
         │ Credit  │
         └─────────┘

Mobile (480px)
Amount:   Payment:
┌─────┬─────────┐
│₱500 │         │
├─────┤ GCash   │
│₱2.5K├─────────┤
├─────┤PayMaya  │
│₱5K  ├─────────┤
├─────┤ Bank    │
│Cust.├─────────┤
│amt  │Credit   │
└─────┴─────────┘
```

---

## Typography Scaling

### Heading Sizes

```
Page Title (h1)
Desktop:  2.5rem (40px)
Tablet:   2.2rem (35px)
Mobile:   1.5rem (24px)

Section Heading (h2)
Desktop:  2rem (32px)
Tablet:   1.8rem (29px)
Mobile:   1.3rem (21px)

Subsection (h3)
Desktop:  1.5rem (24px)
Tablet:   1.3rem (21px)
Mobile:   1.1rem (18px)

Body Text
Desktop:  1.1rem (18px)
Tablet:   1rem (16px)
Mobile:   0.95rem (15px)

Small Text
Desktop:  0.9rem (14px)
Tablet:   0.85rem (14px)
Mobile:   0.8rem (13px)
```

---

## Spacing Adjustments

### Padding Examples

```
Container Padding:
Desktop:  3rem (48px)
Tablet:   2rem (32px)
Mobile:   1rem (16px)

Card Padding:
Desktop:  2.5rem (40px)
Tablet:   1.5rem (24px)
Mobile:   1rem (16px)

Section Margin:
Desktop:  3rem (48px)
Tablet:   2rem (32px)
Mobile:   1.5rem (24px)

Gap Between Items:
Desktop:  2rem (32px)
Tablet:   1.5rem (24px)
Mobile:   1rem (16px)
```

---

## Button & Touch Target Sizing

```
Desktop
┌──────────────────┐
│  Standard Button │
│   44px height    │
│   (satisfies AA) │
└──────────────────┘

Tablet
┌──────────────────────┐
│  Button             │
│   44px height       │
│   (same for touch)  │
└──────────────────────┘

Mobile
┌────────────────┐
│ Full Width     │
│ 44px+ height   │
│ Easy to tap    │
└────────────────┘
```

---

## Responsive Media Query Flow

```
                    CSS Written for Mobile First
                              │
                              ▼
                    Mobile Layout (320-479px)
                    └─ Single column
                    └─ Full width elements
                    └─ Minimal padding
                              │
                              ▼
                    @media (min-width: 480px)
                    Enhance for Tablets/Large Phones
                              │
                              ▼
                    @media (min-width: 768px)
                    Optimize for Tablets/iPad
                              │
                              ▼
                    @media (min-width: 1024px)
                    Enhance for Desktop
                              │
                              ▼
                    @media (min-width: 1200px)
                    Full Desktop Experience
```

---

## Device-Specific Layouts

### iPhone/Android Phone (360-480px)
```
Full-width layout
Single column for everything
Touch-optimized buttons (44px+)
Stackable forms
Minimal nav bar
Readable font sizes
```

### iPad/Tablet (768-1024px)
```
Multi-column where appropriate
Better use of horizontal space
Optimized for portrait & landscape
2-3 column grids possible
Balanced spacing
Enhanced typography
```

### Desktop/Laptop (1200px+)
```
Full multi-column layouts
Maximum 1200-1400px content width
Optimized whitespace
Complex grids possible
Full navigation visible
Larger interactive elements
```

---

## Common Responsive Patterns

### Pattern 1: Stack on Mobile
```
@media (max-width: 768px) {
  .grid {
    grid-template-columns: 1fr;  /* Was: 1fr 1fr; */
  }
}
```

### Pattern 2: Full Width Forms
```
@media (max-width: 768px) {
  input, button, select {
    width: 100%;
  }
}
```

### Pattern 3: Scale Typography
```
@media (max-width: 768px) {
  h1 { font-size: 1.8rem; }  /* Was: 2.5rem */
  p { font-size: 1rem; }     /* Was: 1.1rem */
}
```

### Pattern 4: Adjust Spacing
```
@media (max-width: 768px) {
  .container {
    padding: 1rem;  /* Was: 2rem */
  }
  
  .gap {
    gap: 1rem;      /* Was: 2rem */
  }
}
```

---

## Testing Checklist Visual

```
✓ Mobile Test (480px)
  └─ No horizontal scroll
  └─ Text readable
  └─ Buttons touchable
  └─ Forms usable

✓ Tablet Test (768px)
  └─ Layouts optimized
  └─ Multi-column visible
  └─ Content centered
  └─ Navigation clear

✓ Desktop Test (1200px+)
  └─ Full layouts visible
  └─ Proper spacing
  └─ All features shown
  └─ Professional appearance
```

---

## Responsive Design Hierarchy

```
                    All Devices (0px+)
                    - Base styles
                    - Colors, fonts
                    - Mobile-first
                            │
                ┌───────────┼───────────┐
                ▼           ▼           ▼
            480px+      768px+      1024px+
            Mobile+     Tablet+     Desktop+
            - Enhance   - Columns   - Layouts
            - Grid      - Multi     - Multi
            - Spacing   - Gaps      - Spacing
```

---

## Real-World Breakpoint Usage

### HAPAG-ASA Implementation

**Consistent across all pages:**
```
1. Base mobile: 320-479px
   └─ Single column, full width

2. Tablet breakpoint: 768px
   └─ 2-column layouts available
   └─ Enhanced spacing

3. Large breakpoint: 1024px
   └─ Multi-column optimizations
   └─ Better use of space

4. Desktop: 1200px+
   └─ Full feature set
   └─ Optimal layout
```

---

## Notes for Developers

- Mobile-first CSS means styles cascade and enhance
- Use `@media (max-width: X)` when breaking down
- Use `@media (min-width: X)` when building up
- Test at actual breakpoints, not just between them
- Touch targets should be 44px minimum
- Font sizes should be readable (12px+ on mobile)
- Always include viewport meta tag

---

*Visual reference for HAPAG-ASA responsive design implementation*
