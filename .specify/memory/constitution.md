<!--
Sync Impact Report (Constitution Update)
Version Change: 0.0.0 → 1.0.0
Created: Initial constitution ratification for EIE Website
Modified Principles: N/A (initial version)
Added Sections: All core principles, technology constraints, development workflow, governance
Removed Sections: None
Templates Requiring Updates:
  - ✅ .specify/templates/spec-template.md (will be validated)
  - ✅ .specify/templates/plan-template.md (will be validated)
  - ✅ .specify/templates/tasks-template.md (will be validated)
Follow-up TODOs: None
-->

# EIE Website Constitution

## Core Principles

### I. Professional Presentation First (NON-NEGOTIABLE)

**All content and design must present EIE as a professional, enterprise-level logistics provider:**
- High-quality visual design with consistent branding (blue gradient + orange accents)
- Professional copywriting with no grammatical errors
- Fast page load times (<3 seconds on 4G connection)
- Mobile-responsive design for all devices
- Cross-browser compatibility (Chrome, Safari, Firefox, Edge)
- SEO optimization for business visibility

**Rationale:** This website represents EIE to Canada Post executives and global postal union members. Professional presentation directly impacts business opportunities.

### II. Clear Communication of Capabilities

**Every page must clearly demonstrate EIE's business capabilities:**
- Data-driven proof points (500万包裹/年, 40,000+包裹/日)
- Visual hierarchy emphasizing key differentiators
- Concrete service metrics (99%+ 清关通过率, 2-9天妥投时效)
- Clear call-to-actions for business inquiries
- Transparent service process explanations

**Rationale:** Decision-makers need concrete evidence of capabilities. Vague claims reduce credibility.

### III. Technical Excellence

**The website must be technically sound and maintainable:**
- Clean, semantic HTML5 markup
- Well-structured CSS with consistent naming conventions
- Optimized images (WebP format, proper compression)
- Accessible design (WCAG 2.1 Level AA compliance)
- Valid W3C standards compliance
- Documented code for future maintenance

**Rationale:** Technical excellence ensures reliability, maintainability, and professional credibility.

### IV. Fast Iteration & Deployment

**Development must be optimized for rapid delivery:**
- Static HTML/CSS/JS for maximum simplicity
- No complex build processes or dependencies
- Easy deployment to hosting platforms
- Simple content updates without developer intervention
- Version control for all changes

**Rationale:** 4-day timeline requires streamlined development. Over-engineering risks missing deadline.

### V. Content Accuracy (NON-NEGOTIABLE)

**All business data and claims must be accurate:**
- Verified statistics from actual operations
- Accurate service descriptions matching real capabilities
- Correct contact information and business details
- Up-to-date certification and partnership information
- Honest representation of services (no false claims)

**Rationale:** Misrepresentation to Canada Post executives could damage business relationships and reputation.

## Technology Constraints

**Approved Technology Stack** (must be followed unless constitution is amended):

### Frontend
- **Markup:** HTML5 with semantic elements
- **Styling:** CSS3 with modern features (Grid, Flexbox, Custom Properties)
- **Framework:** Vanilla JavaScript (NO React, Vue, Angular for this project)
- **UI Components:** Custom components based on Global Freight Solutions design inspiration
- **Icons:** SVG icons or icon fonts (Font Awesome, Lucide)
- **Fonts:** Google Fonts or system fonts
- **Animation:** CSS transitions and animations, minimal JavaScript

### Assets
- **Images:** WebP format with JPEG fallback, optimized compression
- **Icons:** SVG format for scalability
- **Logo:** High-resolution SVG format

### Deployment
- **Hosting:** Static hosting (Netlify, Vercel, GitHub Pages, or AWS S3)
- **Domain:** Custom domain with HTTPS
- **Analytics:** Google Analytics for visitor tracking

### Development Tools
- **Version Control:** Git with clear commit messages
- **Code Editor:** Any modern editor with HTML/CSS/JS support
- **Browser DevTools:** For debugging and performance testing
- **Validation:** W3C HTML/CSS Validators
- **Performance:** Lighthouse for performance auditing

## Development Workflow

### Feature Development Process

1. **Specification Phase**
   - Use `/speckit.specify` to create feature specification
   - Reference PRD requirements (EIE_Website_PRD.md)
   - Clarify requirements using `/speckit.clarify` if needed
   - Specify acceptance criteria

2. **Planning Phase**
   - Use `/speckit.plan` to create implementation plan
   - Break down into HTML structure, CSS styling, JavaScript interactions
   - Identify required assets (images, icons)
   - Estimate time required

3. **Implementation Phase**
   - Use `/speckit.tasks` to generate task checklist
   - Implement in order: HTML → CSS → JavaScript
   - Use `/speckit.implement` for guided implementation
   - Test in multiple browsers during development

4. **Quality Assurance Phase**
   - Use `/speckit.checklist` for quality verification
   - Validate HTML/CSS with W3C validators
   - Run Lighthouse performance audit
   - Test responsive design on multiple devices
   - Verify all links and forms work correctly

5. **Deployment Phase**
   - Commit changes with clear messages
   - Deploy to staging environment
   - Final QA testing
   - Deploy to production

### Code Review Requirements

**All code changes must be reviewed for:**
- ✅ Adherence to design specification
- ✅ Mobile responsiveness
- ✅ Cross-browser compatibility
- ✅ Performance optimization
- ✅ Accessibility compliance
- ✅ SEO best practices
- ✅ Code quality and maintainability

### Quality Gates

**No code can be deployed without passing:**
1. W3C HTML/CSS validation (zero errors)
2. Lighthouse score: Performance >90, Accessibility >90, Best Practices >90, SEO >90
3. Mobile-friendly test passing
4. Manual testing on Chrome, Safari, Firefox
5. All forms and links verified working
6. Content accuracy verified against PRD

## Project-Specific Guidelines

### Design Guidelines
- **Primary Color:** Blue gradient (#1e3a8a to #3b82f6)
- **Accent Color:** Orange (#f97316)
- **Typography:** Professional sans-serif fonts (Inter, Open Sans, or similar)
- **Layout:** Left-text, right-image pattern for sections
- **White Space:** Generous padding and margins for readability

### Content Guidelines
- **Tone:** Professional, confident, data-driven
- **Language:** Bilingual ready (English primary, Chinese secondary)
- **Statistics:** Always cite source and update date
- **Images:** High-quality professional photography (warehouses, operations, facilities)

### SEO Requirements
- **Title Tags:** Descriptive, includes key services
- **Meta Descriptions:** Compelling, includes call-to-action
- **Header Tags:** Proper H1-H6 hierarchy
- **Alt Text:** Descriptive for all images
- **Schema Markup:** Organization and Service schema

### Performance Requirements
- **Page Load:** <3 seconds on 4G connection
- **First Contentful Paint:** <1.5 seconds
- **Largest Contentful Paint:** <2.5 seconds
- **Cumulative Layout Shift:** <0.1
- **Image Size:** Maximum 200KB per image
- **Total Page Size:** <3MB including all assets

## Governance

### Constitution Updates

**This constitution can be updated through:**
1. **Minor Updates** (typos, clarifications): Direct commits with clear rationale
2. **Major Updates** (new principles, technology changes): Discussion and team approval required

### Compliance Verification

**Regular checks required:**
- Weekly design review against PRD requirements
- Daily Lighthouse audits during development
- Pre-deployment comprehensive QA checklist

### Exception Process

**Exceptions to this constitution require:**
1. Clear business justification
2. Risk assessment
3. Mitigation plan
4. Documentation of decision

---

**Version:** 1.0.0
**Last Updated:** 2025-11-04
**Next Review:** After initial deployment
**Owner:** Development Team
