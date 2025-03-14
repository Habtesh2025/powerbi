# powerbiPower BI Workspace Admin Best Practices: Marketing Department 

1. Setting Up a Power BI Workspace Properly



Guidelines:



✔ Members can edit Power BI artifacts and add users but cannot remove users.

✔ Admins (Content Team) manage full workspace control, including user removal.

✔ CMO & Marketing Directors remain Viewers, ensuring they can only review reports.



Marketing :



A CMO and Marketing Director need read-only access, while Brand, Digital, and Product Marketing Managers should manage reports and invite new users but cannot remove existing team members.

• Workspace Name: “Marketing Analytics & Performance”

• Roles & Permissions:

• Content Team (Copywriters, Designers, Content Marketing Manager) → Admins (Full control, including adding/removing users)

• Brand Manager, Digital Marketing Manager, Product Marketing Manager → Members (Can edit Power BI artifacts and add users but cannot remove users)

• PR Manager, Event Coordinator → Contributors (Can create and publish reports but cannot manage permissions)

• CMO & Marketing Director → Viewers (Can only view dashboards and reports)

2. Managing Permissions and Access Control



Guidelines:



✔ Members can add users but not remove them.

✔ Admins retain control over user removals to maintain security.

✔ Use Azure AD Groups for streamlined access control.



Marketing :



The Brand Manager (Member) wants to add a new Social Media Coordinator to the workspace but cannot remove existing users.

• User Management Flow:

• Brand Manager (Member) → Adds Social Media Coordinator as a Contributor

• Content Marketing Manager (Admin) → Oversees changes & can remove users if needed

• CMO (Viewer) → No permission changes allowed

3. Ensuring Data Security and Governance



Guidelines:



✔ Row-Level Security (RLS) ensures controlled data access.

✔ CMO & Marketing Directors remain Viewers to prevent accidental edits.

✔ Members can expand access but cannot compromise data security.



Marketing :



The Digital Marketing Manager (Member) can add a new marketing analyst to review ad campaign performance, but cannot remove other existing team members.

• Row-Level Security Setup:

• Content Team (Admins) → Full Access

• Brand Manager, Digital Marketing Manager, Product Marketing Manager → See relevant data

• CMO & Marketing Director → View only high-level KPIs

4. Optimizing Performance and Storage



Guidelines:



✔ Members manage refresh schedules to optimize performance.

✔ Admins enforce quarterly data cleanup.

✔ DirectQuery is used for real-time ad performance insights.



Marketing :



The Product Marketing Manager (Member) updates the refresh frequency for the Sales Funnel Report to prevent unnecessary processing delays.

• Sales Funnel Report Settings:

• Data Source: Google Analytics, CRM System

• Refresh Frequency: Adjusted from daily to every 6 hours

• Managed by: Product Marketing Manager (Member)

5. Managing Reports and Datasets Efficiently



Guidelines:



✔ Members can edit and publish reports.

✔ Admins ensure dataset consistency and security.

✔ Contributors (PR & Event Coordinators) can create dashboards but not manage permissions.



Marketing :



The Digital Marketing Manager (Member) updates the SEO Performance Report to include new keyword rankings, while the Content Team (Admins) ensures consistency across reports.



✔ SEO_Performance_2025.pbix (Updated by Digital Marketing Manager)

✔ Ad_Campaign_Results_2025.pbix (Managed by Brand Manager)

6. Automating Monitoring and Alerts



Guidelines:



✔ Members manage alerts for performance changes.

✔ Admins monitor overall workspace activities.

✔ Data refresh failure notifications are sent to Members & Admins.



Marketing :



If customer engagement rates drop below 5%, the Brand Manager (Member) receives an alert and adjusts content strategy accordingly.

• Alert Setup:

• Metric: Engagement Rate < 5%

• Notification: Email + Microsoft Teams alert

• Response: Adjust marketing strategy

7. Collaboration and Sharing Best Practices



Guidelines:



✔ Members share reports using Power BI Service links.

✔ Teams use Microsoft Teams for dashboard discussions.

✔ Admins ensure Viewers (CMO & Directors) have dashboard access.



Marketing :



Instead of emailing reports, the Product Marketing Manager (Member) shares the Quarterly Product Performance Dashboard in Microsoft Teams.

• Teams Integration:

• Pinned dashboards in Marketing Teams channel

• Comments enabled for discussions

• CMO & Marketing Directors only have Viewer access

8. Regular Maintenance and Housekeeping



Guidelines:



✔ Members oversee quarterly user access reviews (but cannot remove users).

✔ Admins (Content Team) handle workspace cleanup and user removals.

✔ Unused reports are archived.



Marketing :



At the end of Q3, the Digital Marketing Manager (Member) reviews user access and adds a new Performance Analyst to the workspace. However, they cannot remove old users—this requires Admin approval.

• Quarterly Cleanup Checklist:

• Add new team members as needed

• Archive outdated campaign reports

• Ensure dataset refresh schedules are optimized
