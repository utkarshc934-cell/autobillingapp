# OM Logistics Business App

This package provides a unified navigation shell for the existing OM Logistics modules.

## Modules
- Employee Management
- Auto Billing Master Data
- RFQ Control Deck

## Netlify deployment
1. Extract the ZIP.
2. In Netlify, choose **Add new site → Deploy manually**.
3. Drag the extracted folder into the deploy area.
4. Ensure `index.html` is at the published root.

The original module HTML files are retained unchanged inside the package.


## Supabase integration
The shell exposes the authenticated Supabase client to the three modules. Billing, employee imports/edits, RFQ uploads, and monthly employee report persistence attempt cloud synchronization using the existing tables. Keep the tables' JSON `data` column and RLS policies enabled.
