# Mobile Responsiveness Testing Guide

## How to Test Responsive Design

### Method 1: Chrome DevTools (Recommended)
1. Open any HAPAG-ASA page in Chrome
2. Press `F12` to open Developer Tools
3. Click the **device toggle** icon (top-left, looks like a phone/tablet)
4. Select different devices from the dropdown:
   - **iPhone 12** (390x844px) - Android equivalent
   - **iPad** (768x1024px)
   - **Responsive** - Drag to test custom widths

### Method 2: Firefox Developer Tools
1. Press `F12` to open Developer Tools
2. Click **Responsive Design Mode** (Ctrl+Shift+M)
3. Select device from dropdown or manually set width/height

### Method 3: Real Device Testing
1. Access the application on a real Android phone/tablet
2. Access the application on a real iPad
3. Test on desktop at various zoom levels

---

## Responsive Breakpoints to Test

### Mobile (360px - 480px)
**Files to test:**
- `home.html` - Hero card, metrics row should stack
- `donation.html` - Amount grid should be 1 column
- `program.html` - Program cards should be full width
- `profile.html` - Form inputs should stack vertically
- `about.html` - Cards should be single column

**What to verify:**
- ✓ Navigation text is visible and readable
- ✓ No horizontal scrolling
- ✓ Form fields are full width
- ✓ Buttons are easy to tap (large enough)
- ✓ Font sizes are readable without zoom
- ✓ Images scale appropriately

### Tablet (768px - 1024px)
**Files to test:**
- `home.html` - Dashboard grid should be optimized
- `donation.html` - Amount grid should be 2 columns
- `program.html` - Program cards layout should adjust
- `about.html` - Cards layout should adapt

**What to verify:**
- ✓ Layout uses available space well
- ✓ Multi-column layouts visible where needed
- ✓ Content isn't stretched too wide
- ✓ Navigation remains accessible
- ✓ Form spacing is appropriate

### Desktop (1200px+)
**Files to test:**
- All pages should display full layouts
- All features visible and functional

**What to verify:**
- ✓ Full width layouts work correctly
- ✓ Multi-column grids display properly
- ✓ Content max-width is reasonable
- ✓ All interactive elements work
- ✓ No layout issues at extra wide resolutions

---

## Specific Pages to Test

### Home Page (home.html)
- [ ] Navigation adjusts at 1199px, 768px, 480px
- [ ] Hero card padding scales properly
- [ ] Metrics row stacks on mobile
- [ ] Welcome section is full-width on mobile
- [ ] Dashboard grid collapses to single column on tablet
- [ ] All text remains readable
- [ ] Images/icons scale properly

### Donation Page (donation.html)
- [ ] Hero banner padding adjusts
- [ ] Amount selection grid: 3 cols → 2 cols → 1 col
- [ ] Payment methods grid stacks on mobile
- [ ] Form inputs are full width on mobile
- [ ] Donor information form rows stack properly
- [ ] Button is full width on mobile
- [ ] Info box text remains readable

### About Page (about.html)
- [ ] Page title scales appropriately
- [ ] Section cards have proper padding
- [ ] Cards stack properly on mobile
- [ ] Text is readable at all sizes
- [ ] Footer layout adjusts (2 cols → 1 col)
- [ ] Contact info displays well on mobile

### Programs Page (program.html)
- [ ] Program cards grid: 2 cols → 1 col
- [ ] Card content stacks on mobile
- [ ] Buttons are full width on small screens
- [ ] Encourage message text scales
- [ ] Navigation is visible and accessible

### Profile Page (profile.html)
- [ ] Form rows stack: 2 cols → 1 col
- [ ] Section titles scale properly
- [ ] Input fields are full width
- [ ] Buttons are full width and easy to tap
- [ ] Profile header adapts to mobile
- [ ] Form spacing is consistent

### Login Pages (index.html, admin-login.html)
- [ ] Login container grid: 2 cols → 1 col
- [ ] Brand section displays on all screen sizes
- [ ] Form inputs are properly sized
- [ ] Buttons are easy to tap on mobile
- [ ] Background image scales
- [ ] Text remains readable

### Sign Up Page (signup.html)
- [ ] Two-column layout adapts to single column
- [ ] Brand side displays properly on mobile
- [ ] Form fields stack correctly
- [ ] Navigation adjusts
- [ ] All inputs are touch-friendly

---

## Common Issues to Look For

### ❌ Avoid:
- Horizontal scrolling (content exceeding viewport width)
- Text too small to read (< 12px on mobile)
- Buttons too small to tap (< 44px on mobile)
- Content cut off at edges
- Images stretched or distorted
- Form fields overlapping text
- Navigation items crashing together

### ✓ Ensure:
- Proper contrast and readability
- Touch-friendly interactive elements
- Responsive images and icons
- Proper spacing and padding
- Content fits within viewport
- No layout breaks at any width
- Smooth transitions between breakpoints

---

## Media Query Testing Checklist

### At 1199px (Large Desktop)
- [ ] Hero card has adequate padding
- [ ] Dashboard grid shows 2 columns
- [ ] All content visible without scrolling

### At 1024px (Large Tablet)
- [ ] Content fits well
- [ ] Grid layouts adjust
- [ ] No stretched content

### At 768px (Tablet/iPad)
- [ ] Navigation text size changes
- [ ] Payment grid becomes 1 column (donation)
- [ ] Dashboard grid becomes 1 column (home)
- [ ] Form rows become 1 column (profile)

### At 480px (Mobile)
- [ ] All text is readable
- [ ] Form fields full width
- [ ] Buttons full width
- [ ] No horizontal scroll
- [ ] Navigation is accessible

### At 360px (Small Mobile)
- [ ] All text remains readable
- [ ] Navigation still works
- [ ] Content still fits
- [ ] Touch targets adequate

---

## Browser Testing

Test on these browsers and devices:
- [ ] Chrome (Desktop)
- [ ] Firefox (Desktop)
- [ ] Safari (Mac)
- [ ] Chrome Mobile (Android)
- [ ] Safari (iOS/iPad)
- [ ] Samsung Internet (Android)
- [ ] Edge (Desktop/Mobile)

---

## Performance Tips

- Mobile responsiveness improves user experience
- Faster page loads on mobile with optimized layouts
- Better engagement with touch-friendly buttons
- Reduced bounce rate from better mobile experience
- Better SEO rankings (Google favors mobile-responsive)

---

## Quick Reference: CSS Media Queries Used

```css
/* Tablets and iPad */
@media (max-width: 1024px) { ... }

/* Small tablets and large phones */
@media (max-width: 768px) { ... }

/* Mobile phones */
@media (max-width: 480px) { ... }

/* Very small phones */
@media (max-width: 360px) { ... }
```

All breakpoints are consistent across all CSS files (home.css, donation.css, about.css, program.css, profile.css).

---

## Success Indicators

✅ All pages load and display correctly at all breakpoints
✅ No horizontal scrolling at any width
✅ Text is readable without zooming
✅ Forms are usable on mobile
✅ Navigation remains accessible
✅ Images scale properly
✅ Buttons are touch-friendly
✅ Layout adapts smoothly between breakpoints
✅ No errors in browser console
