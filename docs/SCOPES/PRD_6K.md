# Scope Summary v1

This table translates the internal working notes into plain language for client review.
> "*Section, Feature, Page, Block*" are names of the CMS components. For CMS taxonomy and anatomy please refer to: [CMS Hierarchy](https://pages.haxiom.io/@cw-ride-notes/CMS) and [CMS Components Diagram](https://pages.haxiom.io/@cw-ride-notes/COMPONENTS_DIAGRAM)

| Feature | Included in Base Scope | Not Included in Base Scope | Risks, Questions, or Optional Add-Ons |
| --- | --- | --- | --- |
| Simple Admin Studio | One set of admin credentials and a protected admin area | Multi-admin account management is not part of the confirmed base scope | Multiple admin creation is still at risk |
| Simple CMS | Hide sections, hide pages, update copy, update images, update existing blocks, and add pages using three generic page layouts | Rebuilding page layouts or moving blocks around on existing pages is not included | Adding new sections, changing section structure, hiding individual features within a section, or adding new feature types is at risk and may require extra development |
| Existing Site Sections | Existing site sections are included | None identified | Client should confirm whether any current sections can be omitted |
| PDFs: Reports and Briefings | Existing report and briefing PDFs are included | None identified | Embedded PDF previews are at risk |
| Open Data Portal | Existing open data portal content/reference is included | None identified | No open issue noted |
| Donation Payment Processor | Current donation processor remains in scope at the existing fee structure of 5% plus $0.30 per transaction | Migration to Stripe nonprofit pricing is not included in the base scope | Stripe migration remains outside scope unless added later |
| CRM and Database (NationBuilder) | Volunteer and coalition internal forms are included | External forms are not yet defined | Newsletter functionality is at risk, and external form requirements still need clarification |
| Opportunity Pass Info | Opportunity Pass details, links, and PDFs are included | None identified | No open issue noted |
| Featured Video Background | A featured video background is included | Full CMS control for video management is not included in the confirmed base scope | CMS control and storage overhead are at risk; one static video is listed as an optional add-on |
| Site Redesign | Site redesign is included | Advanced animation work is not included in the confirmed base scope | Enhanced styling is a stretch goal; animation effects work is at risk |
| Improved SEO | Not part of the base scope | Full SEO improvements are not included by default | Available as an optional add-on |
| Improved Performance | Performance improvements are included, with image load-time improvements specifically called out | None identified | No open issue noted |
| Improved Site Accessibility | Accessibility improvements are included | None identified | No open issue noted |
| Improved Security | Basic security work is included, including single-admin access control, a protected admin route, and baseline protection against common malware/XSS/DDOS concerns | Additional hardening for cookies, sessions, JWT handling, and broader protected-route work is not included in base scope | Advanced hardening remains outside scope unless added later |
| Temporary Site Maintenance | 14 days of bug fixing and minor updates are included, with a 1 to 2 day turnaround noted | Extended maintenance beyond the included period is not part of the base scope | 30-day maintenance is listed as an optional add-on |
| Social Media | Social media badges and links are included | A live RSS-based social feed is not part of the confirmed base scope | Enhanced social media references and live RSS feed work are at risk |
| Hosting Migration | None confirmed in base scope | Hosting migration away from GoDaddy is not a confirmed included deliverable | Hosting migration is at risk |
| Newsletter / Landing Page Popover | None confirmed in base scope | Not confirmed as an included deliverable | This item is at risk and still needs definition |
| Google Calendar Integration | Not part of the base scope | Calendar integration is not included by default | Available as an optional add-on |
| Site Analytics | Not part of the base scope | Analytics setup and reporting are not included | Could be added later if needed |
| Live Site Logs / Observability | Not part of the base scope | Live logging, observability, and related monitoring are not included | Could be added later if needed |
| Traffic Handling | Not part of the base scope | Traffic spike scaling, traffic-pattern analysis, rage-click analysis, caching strategy, and above-the-fold optimization are not included | Could be added later if traffic planning becomes a priority |

## Additional Notes

| Topic | Client-Facing Note |
| --- | --- |
| Generic page templates | New CMS pages are expected to use three generic layouts rather than custom page-by-page restructuring |
| Layout changes | If a page needs a very different structure, the current workaround is to create a new page from a generic template and hide the old page |
| Possible extra labor | Net-new forms, net-new features, or moving page blocks around may require additional development time. The internal note currently lists this at $150 per day |

