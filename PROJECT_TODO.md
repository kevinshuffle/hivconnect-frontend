# HIV Connect Central NJ - Master Todo List

**Last Updated**: December 5, 2025
**Project Status**: Phase 1 Complete, Phase 2 In Progress
**Total Progress**: ~30% Complete

---

## ✅ Phase 1: Backend Setup & Deployment (COMPLETED)

### Backend Infrastructure ✅
- [x] Initialize PayloadCMS project with Next.js 15
- [x] Configure Cloudflare D1 database
- [x] Set up Cloudflare Workers deployment
- [x] Configure GitHub Actions workflow
- [x] Set up automatic deployment pipeline

### Collections & Schema ✅
- [x] Create Providers collection
- [x] Create Resources collection (scaffolded)
- [x] Create Blog collection (scaffolded)
- [x] Create PDFLibrary collection (scaffolded)
- [x] Create SiteSettings global
- [x] Create Tags collection

### Data Migration ✅
- [x] Export 15 providers from TypeScript
- [x] Import providers into PayloadCMS
- [x] Add 2 additional providers (17 total)
- [x] Verify API endpoints
- [x] Test data integrity

### Frontend Integration ✅
- [x] Create API utility (`/src/lib/api.ts`)
- [x] Update provider directory page
- [x] Update provider detail pages
- [x] Configure environment variables
- [x] Test API integration

### Automatic Rebuilds ✅
- [x] Create webhook system (`triggerFrontendRebuild.ts`)
- [x] Add hooks to Providers collection
- [x] Add hooks to Resources collection
- [x] Add hooks to Blog collection
- [x] Add hooks to PDFLibrary collection
- [x] Fix "await" issue in hooks
- [x] Test automatic rebuilds

### Backend UI Branding ✅
- [x] Design custom landing page
- [x] Add gradient hero section
- [x] Create icon-based action cards
- [x] Add animations and hover effects
- [x] Ensure responsive design
- [x] Deploy to production

---

## ⏳ Phase 2: Content Population & Frontend Pages (IN PROGRESS)

**Estimated Time**: 2-3 weeks
**Priority**: High
**Dependencies**: Phase 1 complete

### Content Creation (0/4 Complete)

#### Resources Collection
- [ ] Add 10-15 HIV testing resources
  - [ ] Testing center locations
  - [ ] Home testing kit information
  - [ ] Testing FAQ documents
  - [ ] Insurance/free testing info
  - [ ] Testing appointment links
- [ ] Add 5-10 treatment resources
  - [ ] Medication guides
  - [ ] Treatment center info
  - [ ] Financial assistance programs
  - [ ] Insurance navigation guides
- [ ] Add 5-10 support resources
  - [ ] Mental health services
  - [ ] Support group information
  - [ ] Housing assistance
  - [ ] Legal aid resources
  - [ ] Transportation help

**Acceptance Criteria**:
- Minimum 20 total resources
- Each resource has title, description, category
- PDFs uploaded or external links provided
- Tags assigned for filtering
- All resources marked as "published"

#### Blog/News Collection
- [ ] Create 5-10 blog posts
  - [ ] HIV Awareness Day announcement
  - [ ] New provider spotlight
  - [ ] Service updates
  - [ ] Health tips and education
  - [ ] Community event announcements
- [ ] Add featured images for each post
- [ ] Write compelling excerpts (200 chars)
- [ ] Assign categories and tags
- [ ] Publish posts

**Acceptance Criteria**:
- Minimum 5 blog posts
- All posts have featured images
- Content is bilingual (English/Spanish) or tagged by language
- Posts cover diverse topics
- All posts marked as "published"

#### PDF Library Collection
- [ ] Upload 10-15 official documents
  - [ ] Planning Council bylaws
  - [ ] Annual reports
  - [ ] Service standards
  - [ ] Consumer rights guides
  - [ ] Application forms
- [ ] Organize by category (Forms, Reports, Guides, Policies)
- [ ] Add version numbers
- [ ] Write descriptions for each PDF

**Acceptance Criteria**:
- Minimum 10 PDFs uploaded
- All PDFs under 25MB each
- Proper categorization
- Version tracking for multi-version docs
- All marked as "current" status

#### SiteSettings Global
- [ ] Configure hotline number
- [ ] Upload organization logo
- [ ] Set footer links
  - [ ] About link
  - [ ] Privacy policy link
  - [ ] Terms of service link
  - [ ] Accessibility link
- [ ] Add social media links
  - [ ] Facebook (if applicable)
  - [ ] Twitter (if applicable)
  - [ ] Instagram (if applicable)
- [ ] Set contact email
- [ ] Configure maintenance mode toggle

**Acceptance Criteria**:
- All fields populated
- Links tested and working
- Logo displays correctly
- Hotline number formatted properly

### Provider Expansion (0/1 Complete)
- [ ] Add 8-13 more providers (target: 25-30 total)
  - [ ] Research additional providers in Middlesex County
  - [ ] Research additional providers in Somerset County
  - [ ] Research additional providers in Hunterdon County
  - [ ] Verify provider information (phone, hours, services)
  - [ ] Obtain coordinates for map display
  - [ ] Import into PayloadCMS
  - [ ] Test on frontend

**Acceptance Criteria**:
- Minimum 25 total providers
- All 3 counties represented
- All providers have complete data
- Coordinates accurate for map
- All providers marked as "active"

### Frontend Blog Pages (0/2 Complete)

#### Blog Listing Page (`/src/pages/blog/index.astro`)
- [ ] Create blog listing page component
- [ ] Fetch blog posts from PayloadCMS API
- [ ] Display posts in grid layout
- [ ] Show featured image, title, excerpt, date
- [ ] Add pagination (10 posts per page)
- [ ] Add category filter
- [ ] Add search functionality
- [ ] Style with Tailwind CSS
- [ ] Add bilingual support (English/Spanish)
- [ ] Test on all devices (desktop, tablet, mobile)

**Acceptance Criteria**:
- Posts load from API successfully
- Pagination works (10 per page)
- Category filter updates results
- Search returns relevant posts
- Responsive on all devices
- SEO meta tags included

#### Blog Detail Page (`/src/pages/blog/[slug].astro`)
- [ ] Create blog detail page component
- [ ] Fetch single post by slug from API
- [ ] Render featured image
- [ ] Render rich text content
- [ ] Display post metadata (date, author, category)
- [ ] Add social sharing buttons
  - [ ] Share on Facebook
  - [ ] Share on Twitter
  - [ ] Copy link to clipboard
- [ ] Add "Related Posts" section (3-5 posts)
- [ ] Add breadcrumb navigation
- [ ] Style with Tailwind CSS
- [ ] Test on all devices

**Acceptance Criteria**:
- Post loads from API successfully
- Rich text renders correctly
- Images display properly
- Social sharing works
- Related posts are relevant
- Responsive on all devices
- SEO meta tags included

### Frontend Resources Page (0/1 Complete)

#### Resources Library Page (`/src/pages/resources/index.astro`)
- [ ] Create resources library page component
- [ ] Fetch resources from PayloadCMS API
- [ ] Display resources in grid/list layout
- [ ] Show title, description, category, icon
- [ ] Add category filter (Testing, Treatment, Support, etc.)
- [ ] Add tag filter
- [ ] Add search functionality
- [ ] Handle PDF downloads from R2
- [ ] Handle external links (open in new tab)
- [ ] Add language filter (English/Spanish/Both)
- [ ] Style with Tailwind CSS
- [ ] Test on all devices

**Acceptance Criteria**:
- Resources load from API successfully
- PDF downloads work correctly
- External links open in new tab
- Category filter updates results
- Search returns relevant resources
- Responsive on all devices
- Accessible for screen readers

---

## 📋 Phase 3: Additional Features (UPCOMING)

**Estimated Time**: 3-4 weeks
**Priority**: Medium
**Dependencies**: Phase 2 complete

### Contact Form Migration (0/2 Complete)
- [ ] Create ContactForm collection in PayloadCMS
- [ ] Add form fields (name, email, phone, message, subject)
- [ ] Add email notification hook (send to admin)
- [ ] Update frontend contact form to POST to PayloadCMS
- [ ] Remove Netlify Forms dependency
- [ ] Test form submission
- [ ] Test email notifications
- [ ] Add spam protection (honeypot or reCAPTCHA)

### Planning Council Application Migration (0/2 Complete)
- [ ] Create PlanningCouncilApplication collection
- [ ] Add all 40+ fields from current form
- [ ] Add multi-step form support
- [ ] Add email notification hook
- [ ] Update frontend form to POST to PayloadCMS
- [ ] Remove Netlify Forms dependency
- [ ] Test multi-step form flow
- [ ] Test data storage and retrieval

### Search Functionality (0/3 Complete)
- [ ] Implement full-text search in PayloadCMS
- [ ] Create global search endpoint (`/api/search`)
- [ ] Add search page on frontend (`/search`)
- [ ] Search across providers, resources, blog posts
- [ ] Add filters (type, category, date)
- [ ] Add autocomplete/suggestions
- [ ] Optimize search performance

### SEO & Analytics (0/4 Complete)
- [ ] Add sitemap generation (automatic from collections)
- [ ] Add robots.txt
- [ ] Configure Open Graph meta tags
- [ ] Add Twitter Card meta tags
- [ ] Set up Google Analytics 4
- [ ] Set up Cloudflare Web Analytics
- [ ] Configure Analytics collection (v2 scaffold)
- [ ] Add privacy-compliant cookie banner (if needed)

---

## 🚀 Phase 4: Production Optimization (FUTURE)

**Estimated Time**: 1-2 weeks
**Priority**: Medium
**Dependencies**: Phase 3 complete

### Performance (0/5 Complete)
- [ ] Optimize images (use Cloudflare Image Resizing)
- [ ] Add API response caching (Cloudflare Cache API)
- [ ] Implement ISR (Incremental Static Regeneration) for blog
- [ ] Reduce build time (currently ~2-3 minutes)
- [ ] Run Lighthouse audit (target: >90 all categories)
- [ ] Optimize bundle size
- [ ] Add lazy loading for images

### Monitoring & Alerts (0/6 Complete)
- [ ] Set up uptime monitoring (UptimeRobot or Pingdom)
- [ ] Configure error logging (Sentry or similar)
- [ ] Set up alert notifications (email/Slack)
- [ ] Monitor API response times
- [ ] Monitor database size
- [ ] Create monitoring dashboard

### Backup & Recovery (0/4 Complete)
- [ ] Implement automatic database backups (daily)
- [ ] Test backup restoration process
- [ ] Document recovery procedures
- [ ] Set up off-site backup storage (if needed)

### Security Hardening (0/5 Complete)
- [ ] Run security audit (Mozilla Observatory)
- [ ] Test with OWASP ZAP
- [ ] Implement rate limiting on API endpoints
- [ ] Add CAPTCHA to public forms
- [ ] Review and tighten CORS policy
- [ ] Set up security monitoring

---

## 🎯 Phase 5: Custom Domain & Launch (FUTURE)

**Estimated Time**: 1 week
**Priority**: Medium
**Dependencies**: Phase 4 complete

### Domain Configuration (0/5 Complete)
- [ ] Purchase custom domain (or use existing)
- [ ] Configure DNS records
  - [ ] A record for `hivconnectcnj.org` → Cloudflare Pages
  - [ ] CNAME for `api.hivconnectcnj.org` → Cloudflare Workers
  - [ ] MX records for email (if needed)
- [ ] Set up SSL certificate (automatic via Cloudflare)
- [ ] Test domain resolution
- [ ] Update environment variables with production domain

### Final Testing (0/6 Complete)
- [ ] Run full QA checklist (see CLAUDE.md)
- [ ] Cross-browser testing (Chrome, Firefox, Safari, Edge)
- [ ] Mobile device testing (iOS, Android)
- [ ] Accessibility audit (axe DevTools, WAVE)
- [ ] Load testing (simulate 100+ concurrent users)
- [ ] Security scan (SecurityHeaders.com, SSL Labs)

### Client Handoff (0/5 Complete)
- [ ] Create client training materials
- [ ] Record video walkthrough of admin UI
- [ ] Create content editor guide
- [ ] Schedule handoff meeting with Terri/MSHTGA staff
- [ ] Provide admin credentials securely
- [ ] Set up support channel (email or Slack)

---

## 🔮 Phase 6: Version 2 Features (2026)

**Estimated Time**: 8-12 weeks (spread across 2026)
**Priority**: Low
**Dependencies**: Phase 5 complete, client feedback

### Events & Calendar (0/5 Complete) - v2
- [ ] Unhide Events collection
- [ ] Unhide Calendar collection
- [ ] Create events listing page (`/events`)
- [ ] Create event detail page (`/events/[slug]`)
- [ ] Add calendar widget
- [ ] Add event registration functionality
- [ ] Add iCal export

### Volunteer/Donor Centers (0/4 Complete) - v2
- [ ] Unhide VolunteerCenters collection
- [ ] Create volunteer opportunities page
- [ ] Create donor centers directory
- [ ] Add volunteer sign-up form
- [ ] Add donation tracking (if applicable)

### Impact Dashboard (0/5 Complete) - v2
- [ ] Unhide ImpactDashboard collection
- [ ] Design dashboard UI
- [ ] Create data visualization components
- [ ] Add metrics tracking (providers served, resources accessed, etc.)
- [ ] Create public impact report page
- [ ] Add export functionality (PDF/CSV)

### Analytics Integration (0/4 Complete) - v2
- [ ] Unhide Analytics collection
- [ ] Integrate Google Analytics data
- [ ] Create analytics dashboard in admin
- [ ] Add page view tracking
- [ ] Add event tracking
- [ ] Create monthly analytics reports

---

## 🐛 Technical Debt & Improvements

### Infrastructure (0/3 Complete)
- [ ] Set up staging environment
  - [ ] Create `hivconnect-cms-staging` D1 database
  - [ ] Create `hivconnect-pdfs-staging` R2 bucket
  - [ ] Deploy backend to staging Worker
  - [ ] Deploy frontend to staging Pages project
  - [ ] Configure staging webhook
- [ ] Implement database migrations strategy
- [ ] Add automated testing (unit + integration)

### Code Quality (0/4 Complete)
- [ ] Add TypeScript types for all API responses
- [ ] Implement error boundaries on frontend
- [ ] Add loading states for async operations
- [ ] Add retry logic for failed API calls

### Developer Experience (0/3 Complete)
- [ ] Create local development setup guide
- [ ] Add pre-commit hooks (linting, formatting)
- [ ] Create component library documentation
- [ ] Add Storybook for UI components (optional)

---

## 📊 Progress Summary

### Overall Progress
- **Phase 1**: ✅ 100% Complete (Backend setup, deployment, branding)
- **Phase 2**: ⏳ 0% Complete (Content population, frontend pages)
- **Phase 3**: ⏳ 0% Complete (Additional features)
- **Phase 4**: ⏳ 0% Complete (Production optimization)
- **Phase 5**: ⏳ 0% Complete (Custom domain, launch)
- **Phase 6**: ⏳ 0% Complete (v2 features for 2026)

### Total Tasks
- **Completed**: 47 tasks
- **In Progress**: 0 tasks
- **Remaining**: 150+ tasks
- **Total Progress**: ~30%

### Next 5 Immediate Tasks (Priority Order)

1. **Add Resources to Resources Collection**
   - File: PayloadCMS Admin → Resources
   - Estimate: 2-3 hours
   - Priority: High
   - Dependency: None

2. **Create Blog Posts in Blog Collection**
   - File: PayloadCMS Admin → Blog
   - Estimate: 2-3 hours
   - Priority: High
   - Dependency: None

3. **Upload PDFs to PDFLibrary Collection**
   - File: PayloadCMS Admin → PDFLibrary
   - Estimate: 1-2 hours
   - Priority: High
   - Dependency: None

4. **Build Blog Listing Page**
   - File: `/src/pages/blog/index.astro`
   - Estimate: 3-4 hours
   - Priority: High
   - Dependency: Task #2 (blog posts created)

5. **Build Blog Detail Page**
   - File: `/src/pages/blog/[slug].astro`
   - Estimate: 2-3 hours
   - Priority: High
   - Dependency: Task #4 (blog listing page)

---

## 🎯 Success Metrics

### Phase 2 Completion Criteria
- [ ] Minimum 20 resources in Resources collection
- [ ] Minimum 5 blog posts in Blog collection
- [ ] Minimum 10 PDFs in PDFLibrary collection
- [ ] SiteSettings fully configured
- [ ] Minimum 25 total providers
- [ ] `/blog` page live and functional
- [ ] `/blog/[slug]` page live and functional
- [ ] `/resources` page live and functional

### Phase 3 Completion Criteria
- [ ] Contact form submitting to PayloadCMS
- [ ] Planning Council application submitting to PayloadCMS
- [ ] Global search working across all content
- [ ] SEO meta tags on all pages
- [ ] Analytics tracking active

### Production Launch Criteria
- [ ] Custom domain configured
- [ ] All QA checklists passed
- [ ] Client training completed
- [ ] Monitoring and alerts active
- [ ] Backup system in place
- [ ] Security audit passed

---

## 📝 Notes for Next Session

### Start Here
1. Read `/Users/kevincan/Desktop/ShuffleSEO/mshtga/PROJECT_STATUS.md`
2. Read `/Users/kevincan/Desktop/ShuffleSEO/mshtga/SESSION_2025-12-05.md`
3. Review this todo list
4. Check deployment status (all systems should be live)

### Quick Start Commands
```bash
# Backend (local)
cd /Users/kevincan/Desktop/ShuffleSEO/mshtga-backend-workers
pnpm dev
# → http://localhost:3000/admin

# Frontend (local)
cd /Users/kevincan/Desktop/ShuffleSEO/mshtga
npm run dev
# → http://localhost:4321

# Check deployment status
gh run list  # Backend deployments
# Frontend: https://dash.cloudflare.com → Pages → hivconnect-frontend
```

### Recommended Next Task
**Start with content population** (Phase 2):
1. Log into PayloadCMS admin: https://hivconnect-backend.shuffle-seo.workers.dev/admin
2. Add 5-10 resources to Resources collection
3. Add 2-3 blog posts to Blog collection
4. Test automatic frontend rebuild
5. Verify content displays on frontend

This will provide content for building the frontend pages.

---

**Last Updated**: December 5, 2025
**Maintained By**: Kevin / Shuffle SEO
**Project Status**: Active Development
