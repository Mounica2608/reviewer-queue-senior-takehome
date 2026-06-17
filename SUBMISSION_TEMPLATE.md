# \# Submission

# 

# 

# \## Summary of changes

# Built a Vue (Vue.js 3) reviewer queue UI with full workflow support. Improved frontend state handling, action validation, and API integration to ensure correct review lifecycle behavior.

# \## Bugs fixed

# Fixed inconsistent item selection when list updates

# Fixed invalid action execution by enforcing status-based button rules

# Improved error handling for API failures

# Fixed stale UI updates after performing actions

# \## Product/UX decisions

# Disabled workflow actions based on item status (unassigned vs in\_review)

# Auto-refresh queue after every action to keep UI consistent

# Kept single-item detail view for focus-driven review workflow

# Clear visual separation between queue list and detail panel

# \## Tests added

# Verified claim action only works for unassigned items

# Verified approve/reject/escalate only work for in\_review items

# Tested API failure handling (network + bad response)

# Tested UI state sync after multiple actions

# \## Known gaps

# No pagination for large review queues

# No optimistic UI updates (relies on refetch)

# No role-based access control (single reviewer only)

# No backend retry strategy on failed actions

# \## Files changed and why

# frontend/src/App.vue → core UI logic, action handling, state sync fixes

# frontend/src/api.ts → improved error handling for better debugging UX

# frontend/src/styles.css → no major changes required (kept minimal UI styling)

# 

# 

# \## AI assistance used

# i haven't use this ai during this home assessment.

# 

