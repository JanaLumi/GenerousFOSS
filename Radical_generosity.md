AI Collaboration Checklist with Practical Examples
Built-In Scaffolding & Onboarding
 * [ ] Enforce persistent progressive discovery
   * How it works: Instead of dumping a user into a full-featured interface on day one or hiding tools behind a 40-page PDF manual, the software presents a simplified, guided mode. Over 30 to 90 days, advanced options surface naturally as core tasks are mastered.
   * Example: In an ERP inventory module, a new user sees only three primary actions (Receive Goods, Check Stock, Dispatch Order). As they complete orders, secondary fields like Batch Tracking and Customs Codes unlock with contextual visual callouts explaining their function directly on screen.
 * [ ] Architect 'Zero-Manual' primary workflows
   * How it works: Core end-to-end tasks are designed as fully self-contained visual flows. Every inputs, validation step, and output action occurs sequentially within the view so the user never has to leave to check external documentation or search a forum.
   * Example: In a month-end accounting close app, the interface displays a visual step-through tracker: Step 1: Upload Bank Statement \rightarrow Step 2: Reconcile Unmatched Line Items \rightarrow Step 3: Generate P&L Summary. The reconciliation step automatically highlights potential matches side-by-side with confidence scores, eliminating manual lookup tables.
 * [ ] Integrate structural safeguards over error messages
   * How it works: When a user inputs invalid data or misses a required step, the system avoids cryptically blocking them (e.g., "Error 403: Invalid Payload"). Instead, it visually identifies the gap, explains the issue in plain language, and offers a single-click resolution.
   * Example: When entering a Digital Product Passport (DPP) material weight, if the total component percentages equal 94% instead of 100%, the app displays a highlighted warning box: "Total weight is short by 6%. Would you like to attribute the remaining balance to Unspecified Waste or edit the alloy components?" with two direct buttons.
Contextual Signposting & Wayfinding
 * [ ] Surface controls dynamically based on active intent
   * How it works: The interface monitors the user's current task state and renders only the controls relevant to the immediate next step, keeping the workspace clear of irrelevant icons.
   * Example: In a fluid/production balancing tool, when selecting a raw material tank from the dashboard, the top toolbar dynamically converts to display only tank-specific actions (Adjust Flow Rate, Recalibrate Sensor, Drain Tank), rather than keeping 80 generic toolbar icons visible simultaneously.
 * [ ] Eliminate deep nested menus
   * How it works: Avoid hiding core functionality three or four layers deep in dropdown trees (e.g., Settings > Compliance > Sustainability > LCA Export). High-frequency tools are promoted to contextual action bars or floating quick-access panels.
   * Example: In an auditing tool, hovering over any row in a balance sheet reveals an inline action bar with direct buttons for Attach Receipt, Add Audit Note, and Flag Line Item, bypassing the traditional right-click sub-menu navigation.
 * [ ] Maintain visual 'Airflow' and contrast hierarchy
   * How it works: Use deliberate spatial padding, clear font scale differentials, and visual grouping to prevent "data claustrophobia." Important data points are given high visual weight, while secondary metrics sit quietly until hovered or focused.
   * Example: An executive financial dashboard presents the core metric (Net Cash Flow) in a prominent, large font with ample surrounding white space. Supporting details (individual bank accounts and pending transfers) sit in a lower-contrast, collapsible drawer beneath it, keeping the screen readable at a glance.
Workflow Continuity & Koti-tonttu Feedback
 * [ ] Build inline intent-to-action paths
   * How it works: Complex multi-system processes are connected into a single unbroken linear timeline, preventing the user from needing to jump between separate tabs or modules to complete one job.
   * Example: When creating a purchase order in a manufacturing ERP, the UI automatically embeds the supplier's real-time stock levels, lead times, and carbon intensity metrics directly inside the line-item view, so the buyer doesn't have to open a separate inventory tab or LCA spreadsheet.
 * [ ] Audit for self-documenting interface state
   * How it works: Every field, button, and status indicator clearly describes its function, its input requirements, and what consequence clicking it will have, removing the need for external FAQs or help tickets.
   * Example: A button labeled "Archive Fiscal Year" features sub-text directly beneath it reading: "Calculates final retained earnings, locks 2025 transactions from edits, and generates read-only compliance PDFs for auditing."
### Mechanics-to-Accessibility Audit
 * [ ] Eliminate fine-motor dependencies
   * Replace hover-triggered sub-menus with sticky or contextually surfaced action bars with minimum 44px touch/click targets.
 * [ ] Enforce non-destructive focus states
   * Ensure inline guidance and scaffolding keep keyboard/screen reader focus in logical order without modal focus traps.
 * [ ] Provide dual-channel visual feedback
   * Ensure every visual cue (status, priority, warning) uses spatial position, text, or shape in addition to color.
 * [ ] Maintain zoom and reflow stability
   * Test high-density views (tables, ERP balance sheets) at 200% text zoom to ensure layouts reflow smoothly without horizontal scroll collisions.
