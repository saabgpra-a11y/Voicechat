# Voice Chat Social App - Design Guidelines

## Design Approach

**Reference-Based Approach** drawing inspiration from social voice platforms like Yalla, Bigo Live, and Discord, combined with gaming UI elements for the gift/reward systems. This is an experience-focused, socially-driven platform where visual appeal and emotional engagement are paramount.

## Core Design Principles

1. **Social Energy**: Bold, vibrant aesthetics that convey liveliness and social connection
2. **Status & Achievement**: Clear visual hierarchy for user levels, badges, and rewards
3. **Immersive Rooms**: Voice rooms should feel like virtual gathering spaces
4. **Instant Gratification**: Visual feedback for all social interactions (gifts, reactions, entry/exit)

---

## Color Palette

### Primary Colors (Dark Mode - Default)
- **Background Base**: 220 25% 10% (deep navy-purple)
- **Surface**: 220 20% 15% (elevated surfaces, cards)
- **Surface Elevated**: 220 18% 20% (modals, active rooms)

### Accent Colors
- **Primary Brand**: 280 80% 60% (vibrant purple - for CTAs, active states)
- **Secondary**: 340 75% 55% (pink-magenta - for gifts, special features)
- **Success/Coins**: 45 90% 55% (golden yellow - for coins, rewards)
- **Live Indicator**: 0 85% 60% (red - for live rooms, active status)

### Gradients
- **Hero/Premium**: 280 80% 60% to 340 75% 55% (purple to pink)
- **Coin/Reward**: 40 90% 50% to 50 95% 60% (gold gradient)
- **VIP Badge**: 280 70% 50% to 260 80% 65% (royal purple)

### Light Mode
- **Background**: 240 20% 98%
- **Surface**: 0 0% 100%
- **Text Primary**: 220 25% 15%
- Maintain same accent colors for consistency

---

## Typography

### Font Families
- **Primary**: 'Poppins' (Google Fonts) - Modern, friendly, great for UI
- **Display/Numbers**: 'Space Grotesk' (Google Fonts) - Bold headers, coin counts
- **Accent**: 'Inter' (Google Fonts) - Body text, descriptions

### Type Scale
- **Hero/Room Names**: text-4xl to text-5xl, font-bold (Space Grotesk)
- **Section Headers**: text-2xl to text-3xl, font-semibold (Poppins)
- **User Names**: text-lg, font-medium (Poppins)
- **Body**: text-base, font-normal (Inter)
- **Captions/Meta**: text-sm, font-normal (Inter)
- **Coin Counts**: text-xl to text-2xl, font-bold (Space Grotesk)

---

## Layout System

### Spacing Primitives
Use Tailwind units: **2, 4, 6, 8, 12, 16** for consistent rhythm
- Tight spacing: p-2, gap-2 (within components)
- Standard spacing: p-4, gap-4 (between elements)
- Section spacing: p-6 to p-8, gap-6 to gap-8
- Large spacing: p-12 to p-16 (between major sections)

### Grid Structure
- **Room Grid**: grid-cols-1 md:grid-cols-2 lg:grid-cols-3 for room cards
- **User Avatars in Room**: Circular layout, max 9 visible with "+X more" indicator
- **Leaderboard**: Single column, full-width cards with rank badges
- **Gift Gallery**: grid-cols-3 md:grid-cols-4 lg:grid-cols-5 for gift selection

### Container Widths
- **Main Content**: max-w-7xl mx-auto (dashboard, rooms list)
- **Room View**: max-w-6xl mx-auto (active room interface)
- **Modals**: max-w-2xl (profile, settings)
- **Side Panels**: w-80 (user list, chat)

---

## Component Library

### Navigation
- **Top Nav**: Sticky header with logo, coins balance (with icon), profile avatar, notification bell
- **Tab Bar**: Rounded pill-style tabs with active gradient background
- **Mobile Bottom Nav**: Fixed bottom bar with 4-5 main actions (Home, Explore, Create Room, Wallet, Profile)

### Room Cards (List View)
- **Card Style**: Elevated cards with subtle border glow on hover
- **Layout**: Room image/banner at top, host avatar overlapping bottom edge, room name, user count with avatars, "Join" button with gradient
- **Live Indicator**: Pulsing red dot with "LIVE" badge in top-right corner
- **Capacity Display**: "8/20 users" with mini avatar stack

### Active Room Interface
- **Participant Display**: Circular avatars arranged in arc/circular pattern, host in center/top with crown icon
- **Speaking Indicator**: Animated ring around avatar when speaking (green pulse)
- **Layout**: Main room view occupies 70% width, right sidebar 30% for chat/gifts
- **Control Bar**: Bottom fixed bar with mic toggle, speaker toggle, send gift, leave room buttons

### Gift System
- **Gift Grid**: Colorful icons with coin cost below, hover to preview animation
- **Categories**: Tabs for "Popular", "Romantic", "Fun", "VIP" gifts
- **Send Animation**: Full-screen animated effect when gift sent (roses falling, hearts floating, etc.)
- **Gift Badge**: Small overlay on avatar showing recent gift received

### User Profiles
- **Profile Card**: Large avatar with level ring/border, username, level number, badges row
- **Stats Grid**: 3-column grid showing "Coins Earned", "Gifts Received", "Rooms Hosted"
- **Badge Collection**: Horizontal scrollable gallery of earned badges
- **VIP Indicator**: Special border glow/animation for VIP users

### Leaderboard
- **Rank Display**: Large numbers 1-10 with medal icons for top 3 (gold, silver, bronze)
- **User Row**: Rank number, avatar, username, stats (coins/gifts), progress bar showing relative standing
- **Filter Tabs**: "Daily", "Weekly", "All Time", "Friends"

### Wallet/Coins
- **Balance Display**: Large coin count with icon in top nav and dedicated wallet page
- **Recharge Cards**: Package cards showing coin amounts, bonus indicators, and price
- **Transaction History**: List of recent earnings/spending with icons

### Daily Rewards
- **Calendar Grid**: 7-day grid showing checked days, today highlighted, rewards preview
- **Claim Button**: Prominent gradient button when reward available
- **Streak Counter**: Fire icon with days count

### Badges & Levels
- **Badge Design**: Circular or shield-shaped, colorful with icons
- **Level Progress**: Circular or horizontal progress bar around/below avatar
- **Achievement Toast**: Bottom-right notification when badge earned

---

## Images

### Hero Section (Marketing/Landing)
- **Large Hero Image**: Full-width gradient overlay image showing diverse group of people enjoying voice chat, colorful headphones, vibrant social atmosphere
- **Placement**: Top of landing page, 80vh height
- **Style**: Modern, diverse, energetic photography with purple/pink gradient overlay

### Room Banners
- **Dynamic Backgrounds**: Each room can have custom background image or gradient
- **Style**: Abstract patterns, gaming themes, music vibes, or user-uploaded images
- **Treatment**: Subtle blur or overlay to ensure text readability

### Gift Icons
- **Illustration Style**: Playful 3D-style illustrations or animated SVGs
- **Categories**: Roses, hearts, crowns, diamonds, sports items, emojis
- **Source**: Icon libraries with colorful, premium feel

### Profile Avatars
- **User Uploads**: Circular crop with border indicating level/VIP status
- **Fallback**: Colorful gradient avatars with initials for users without photos
- **Special Effects**: Glow/shimmer for VIP users, animated borders for hosts

---

## Animations & Micro-interactions

**Use Sparingly - Only for Key Moments:**

1. **Gift Sending**: 1-2 second full-screen animation (hearts, sparkles, confetti based on gift type)
2. **Speaking Pulse**: Gentle ring animation around active speaker's avatar
3. **Live Indicator**: Subtle pulsing animation on "LIVE" badges
4. **Room Entry**: Brief fade-in for new user avatars appearing
5. **Level Up**: Celebratory burst animation with badge/level display
6. **Hover States**: Subtle lift/scale on interactive cards (room cards, gift icons)

**Avoid**: Excessive parallax, constant floating animations, distracting background movements

---

## Responsive Behavior

### Desktop (lg:)
- Multi-column room grids (3 columns)
- Side-by-side room view + chat panel
- Expanded navigation with labels
- Larger avatars and UI elements

### Tablet (md:)
- 2-column room grids
- Collapsible side panel (chat overlay)
- Compact navigation

### Mobile (base)
- Single column layouts
- Full-screen room view with swipe-up chat drawer
- Bottom navigation bar
- Simplified gift selector (modal)
- Larger touch targets (min 44px)

---

## Accessibility

- **Dark Mode**: Primary mode with proper contrast ratios (WCAG AA)
- **Light Mode**: Available as toggle with consistent accent colors
- **Focus States**: Visible keyboard focus indicators (2px accent color ring)
- **Icon Labels**: All icon-only buttons include aria-labels
- **Live Regions**: Announce room status changes, new users entering

---

## Visual Hierarchy Priority

1. **Room Status (Live/Active)** - Most prominent
2. **Call-to-Action (Join/Send Gift)** - High contrast, gradient buttons
3. **User Profiles/Avatars** - Medium prominence with clear labels
4. **Meta Information (counts, stats)** - Lower prominence, subtle styling
5. **Background Elements** - Minimal, support primary content