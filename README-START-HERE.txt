LUMIERE — DYNAMIC TEMPLATE SYSTEM (TEST RELEASE)

WHAT CHANGED
- Main website dynamically recognizes template IDs 31, 32, 33, etc. from Firestore siteSettings/public.
- New templates appear only if they have a valid HTTPS published URL AND Gallery visibility = Published.
- New templates can be Classic or VIP and Royal / Floral / Minimal.
- Existing original templates are preserved by default.
- Preview photos, thumbnail and background uploads continue through the connected Supabase account.
- No new database tables, or public bucket write policies, are required.

INSTALLATION
1) GitHub Pages Manager: replace the OLD index.html + manager.html with the NEW manager package from this release.
2) Cloudflare Main website: deploy the MAIN ZIP as a new test deployment before replacing production.
3) Manager > Template Links > Add Template Link. Fill title, subtitle, and HTTPS URL of hosted 31.html.
4) Select category and package access. Gallery visibility: Draft until ready.
5) Save/Publish. Go to Template Customize, select #31, upload thumbnail and optional background (Supabase login), then Save & Publish.
6) Return to Template Links: set Gallery visibility to Published, Publish Changes.
7) Refresh main website: Template #31 should appear with its thumbnail and have a working full preview.

CAUTION
- New HTML templates must be hosted separately (e.g. Cloudflare) before adding the URL. These ZIPs do not include the new 31.html.
- VIP access continues using the existing plan gating, whose wording may still refer to the old 30 templates.
- Live cloud authentication, Firestore security rules, and end-to-end purchase/RSVP flows have not been remotely verified.
- Preserve your previous deployed files as a backup. Test with a new template before updating production.
