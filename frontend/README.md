# MedTech Compliance SaaS Platform - Frontend

A **futuristic, modern, and minimalistic** compliance management platform for medical device startups. Built with Next.js 16, Tailwind CSS 4, GSAP animations, and stunning visual effects.

## 🎨 Design Philosophy

- **Minimalistic & Clean**: Focus on content with ample white space
- **Futuristic**: Modern animations, glassmorphism effects, and smooth transitions
- **Accessible**: WCAG compliant with proper contrast ratios
- **Responsive**: Mobile-first design that works beautifully on all devices
- **Fast**: Optimized performance with lazy loading and code splitting

## 🚀 Tech Stack

- **Framework**: Next.js 16 (App Router)
- **Styling**: Tailwind CSS 4
- **Animations**: 
  - GSAP for advanced scroll animations
  - Framer Motion for component animations
  - Custom CSS animations for special effects
- **Typography**: 
  - Helvetica Neue (primary)
  - Almarai (secondary)
- **Icons**: Lucide React
- **Language**: TypeScript

## 🎨 Color Palette

```css
- Fresh Green: #42C96F (RGB: 66,201,111)
- Deep Teal: #038262 (RGB: 3,130,98)
- Soft Lime: #9ACF0D (RGB: 154,207,13)
- Pale Aqua: #E6F2F1 (RGB: 230,242,241)
- Slate Gray: #6B8C89 (RGB: 107,140,137)
- Forest Green: #30403E (RGB: 48,64,62)
```

## 📁 Project Structure

```
frontend/
├── src/
│   ├── app/                    # Next.js App Router pages
│   │   ├── (auth)/            # Authentication pages
│   │   │   ├── login/
│   │   │   └── signup/
│   │   ├── dashboard/         # Dashboard pages
│   │   │   ├── page.tsx       # Main dashboard
│   │   │   ├── checklist/     # Compliance checklists
│   │   │   ├── documents/     # Document management
│   │   │   ├── templates/     # Templates library
│   │   │   ├── ai-assistant/  # AI chat interface
│   │   │   ├── alerts/        # Notifications & alerts
│   │   │   └── settings/      # Settings page
│   │   ├── onboarding/        # User onboarding flow
│   │   ├── page.tsx           # Landing page
│   │   ├── layout.tsx         # Root layout
│   │   └── globals.css        # Global styles
│   ├── components/
│   │   ├── animations/        # Animation components
│   │   │   ├── FadeIn.tsx
│   │   │   ├── ScrollReveal.tsx
│   │   │   ├── ParallaxText.tsx
│   │   │   └── MagneticButton.tsx
│   │   ├── effects/           # Special effects
│   │   │   ├── GridBackground.tsx
│   │   │   └── FloatingElements.tsx
│   │   ├── layout/            # Layout components
│   │   │   ├── Navbar.tsx
│   │   │   ├── Sidebar.tsx
│   │   │   └── Footer.tsx
│   │   └── ui/                # UI components
│   │       ├── Button.tsx
│   │       ├── Card.tsx
│   │       ├── Badge.tsx
│   │       ├── Input.tsx
│   │       ├── StatCard.tsx
│   │       ├── ProgressBar.tsx
│   │       └── Tooltip.tsx
│   └── public/
│       ├── almarai-webfont/   # Almarai font files
│       └── helvetica-neue-5/  # Helvetica Neue font files
```

## ✨ Key Features

### 1. Landing Page
- Hero section with animated gradient backgrounds
- Feature showcase with hover effects
- Statistics section with animated counters
- Problem-solution narrative
- Testimonials with glassmorphism cards
- Pricing comparison table
- Responsive design for all devices

### 2. Dashboard
- **Overview**: Real-time compliance metrics
- **Regulation Progress**: Visual progress tracking
- **Recent Activity**: Timeline of actions
- **Weekly Activity Chart**: Animated bar chart
- **Team Members**: Live status indicators
- **Upcoming Deadlines**: Priority-based task list
- **Critical Alerts**: Important notifications

### 3. Compliance Checklists
- Multi-regulation support (FDA, ISO, EU MDR, HIPAA)
- Expandable sections
- Task status tracking
- Document linking
- Team assignment
- Priority levels
- Progress visualization

### 4. Document Management
- Folder-based organization
- Grid and list view modes
- Advanced search and filtering
- File type indicators
- Version control
- Status badges (Draft, In Review, Approved)
- Storage usage tracking

### 5. AI Assistant
- Chat interface with message history
- Quick prompt suggestions
- Source citations
- Real-time typing indicators
- Markdown support
- Copy, like/dislike, regenerate options

### 6. Templates Library
- Pre-built compliance templates
- Category filtering
- Difficulty levels
- Regulation tags
- Download statistics
- Preview and download options

### 7. Alerts & Notifications
- Regulatory updates
- Deadline reminders
- Team activity
- System notifications
- Priority-based filtering
- Read/unread status

### 8. Settings
- Company profile management
- Account settings
- Notification preferences
- Regulation selection
- Security settings (2FA, sessions)
- Billing management

## 🎯 Animation Features

### GSAP Animations
- **Scroll-triggered animations**: Elements fade and slide in as you scroll
- **Parallax effects**: Background elements move at different speeds
- **Magnetic buttons**: Buttons follow cursor movement
- **Chart animations**: Bars and progress indicators animate on load

### Framer Motion
- **Page transitions**: Smooth transitions between routes
- **Component animations**: Fade, slide, and scale effects
- **Gesture animations**: Interactive hover and click states

### CSS Animations
- **Gradient animations**: Animated color gradients
- **Pulse effects**: Attention-grabbing pulse animations
- **Shimmer effects**: Text and element shimmer effects
- **Float animations**: Gentle floating elements

## 🔧 Custom Utilities

### Tailwind Classes
```css
.glass-panel       - Glassmorphism effect
.glass-card        - Alternative glass effect
.text-gradient     - Gradient text effect
.hover-lift        - Lift on hover
.animate-float     - Floating animation
.animate-glow      - Glowing effect
.text-shimmer      - Shimmer text effect
.perspective-card  - 3D perspective on hover
```

## 📱 Responsive Design

- **Mobile**: < 768px (Hamburger menu, stacked layout)
- **Tablet**: 768px - 1024px (Collapsible sidebar)
- **Desktop**: > 1024px (Full sidebar, multi-column layouts)

## 🚀 Getting Started

### Prerequisites
- Node.js 20+ (recommended)
- npm or yarn

### Installation

```bash
# Navigate to frontend directory
cd frontend

# Install dependencies
npm install

# Run development server
npm run dev

# Build for production
npm run build

# Start production server
npm start
```

### Development Server
Open [http://localhost:3000](http://localhost:3000) in your browser.

## 🎨 Component Usage Examples

### Button Component
```tsx
import { Button } from "@/components/ui/Button";

<Button variant="primary" size="lg">
  Click Me
</Button>
```

**Variants**: `primary`, `secondary`, `outline`, `ghost`  
**Sizes**: `sm`, `md`, `lg`

### Card Component
```tsx
import { Card } from "@/components/ui/Card";

<Card hoverEffect className="p-6">
  <h3>Card Title</h3>
  <p>Card content...</p>
</Card>
```

### Animation Components
```tsx
import { FadeIn } from "@/components/animations/FadeIn";
import { ScrollReveal } from "@/components/animations/ScrollReveal";

<FadeIn direction="up" delay={0.2}>
  <div>Animated content</div>
</FadeIn>

<ScrollReveal scale blur>
  <div>Scroll-triggered content</div>
</ScrollReveal>
```

### Stat Card
```tsx
import { StatCard } from "@/components/ui/StatCard";
import { TrendingUp } from "lucide-react";

<StatCard
  title="Total Users"
  value="1,234"
  icon={TrendingUp}
  trend={{ value: 12.5, isPositive: true }}
  iconColor="text-freshGreen"
/>
```

### Progress Bar
```tsx
import { ProgressBar } from "@/components/ui/ProgressBar";

<ProgressBar
  value={75}
  max={100}
  showLabel
  animated
  color="success"
/>
```

## 🎭 Design Patterns

### Glass Morphism
Used throughout for cards and panels to create depth and modern aesthetic.

### Gradient Backgrounds
Subtle animated gradients for visual interest without overwhelming content.

### Micro-interactions
Every interactive element has smooth hover, active, and focus states.

### Consistent Spacing
8px grid system for consistent spacing and alignment.

### Typography Hierarchy
Clear hierarchy with consistent font sizes and weights.

## 🔒 Security Features

- Input validation on all forms
- CSRF protection
- Secure session management
- 2FA support (UI ready)
- Audit logging visualization

## ♿ Accessibility

- Semantic HTML throughout
- ARIA labels where needed
- Keyboard navigation support
- Focus indicators
- Color contrast compliance (WCAG AA)
- Screen reader friendly

## 🎯 Performance Optimizations

- Code splitting with Next.js dynamic imports
- Image optimization with Next.js Image component
- Lazy loading for below-the-fold content
- Optimized fonts with font-display: swap
- CSS-in-JS with Tailwind for minimal CSS
- GSAP animations optimized for 60fps

## 📝 Hardcoded Data

All pages use hardcoded data for demonstration purposes:
- User: John Doe (john@medtech.inc)
- Company: MedTech Innovations Inc.
- Team members: Sarah Chen, Michael Rodriguez, Emily Watson
- Various documents, checklists, and templates

## 🌐 Browser Support

- Chrome (latest 2 versions)
- Firefox (latest 2 versions)
- Safari (latest 2 versions)
- Edge (latest 2 versions)

## 📄 License

Proprietary - All rights reserved

## 👥 Credits

Built with ❤️ using modern web technologies.

## 🚀 Future Enhancements

- [ ] Real backend integration
- [ ] WebSocket for real-time updates
- [ ] Advanced search with Algolia
- [ ] PDF viewer for documents
- [ ] Drag-and-drop file upload
- [ ] Collaborative editing
- [ ] Export to PDF/Excel
- [ ] Dark mode support
- [ ] Multi-language support

---

**Note**: This is a frontend demonstration with hardcoded data. Backend integration is required for production use.
