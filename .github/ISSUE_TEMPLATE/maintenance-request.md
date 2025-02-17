---
name: Maintenance Request
about: Report
title: ''
labels: ''
assignees: ''

---

name: Maintenance Request
description: Use this template to report a facility maintenance issue.
title: "[MAINTENANCE REQUEST] - Brief Issue Description"
labels: ["Routine Maintenance", "Urgent Repair", "Pending Approval"]
assignees: []
body:
  - type: markdown
    attributes:
      value: "## Maintenance Request Form\nPlease provide the details of the issue below."

  - type: input
    id: location
    attributes:
      label: "Location"
      description: "Where is the issue located?"
      placeholder: "e.g., Main Hallway, Room 205, Parking Lot"

  - type: textarea
    id: description
    attributes:
      label: "Issue Description"
      description: "Describe the issue in detail."
      placeholder: "The AC unit in Room 205 is not cooling properly."

  - type: dropdown
    id: priority
    attributes:
      label: "Priority Level"
      description: "How urgent is this request?"
      options:
        - Low (Routine Maintenance)
        - Medium (Needs Attention)
        - High (Urgent Repair)

  - type: input
    id: reported_by
    attributes:
      label: "Reported By"
      description: "Who is reporting this issue?"
      placeholder: "John Doe"

  - type: date
    id: report_date
    attributes:
      label: "Date Reported"
      description: "When was this issue reported?"
      
  - type: textarea
    id: additional_notes
    attributes:
      label: "Additional Notes"
      description: "Any extra information?"
      placeholder: "Include any relevant photos or past repairs if applicable."
