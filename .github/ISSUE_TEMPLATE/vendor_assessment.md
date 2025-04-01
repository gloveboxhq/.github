name: Vendor Security Assessment
description: Vendor Security Accessment Form
title: "[VENDOR-ASSESS]: (FILL IN HERE)"
labels: requires-approval
assignees: arolek-glovebox, sethmoeckel-glovebox
body:
  - type: textarea
    id: access_description
    attributes:
      label: Describe the level of access this vendor will have to the GloveBox system
    validations:
      required: true

  - type: textarea
    id: soc2_report_link
    attributes:
      label: Provide a link to the vendors SOC2 report
    validations:
      required: true

  - type: textarea
    id: vendor_name
    attributes:
      label: Specify the vendor name
    validations:
      required: true

  - type: textarea
    id: website
    attributes:
      label: Specify the vendor website
    validations:
      required: true

  - type: textarea
    id: contact
    attributes:
      label: Specify the vendor primary contact name and title
    validations:
      required: true

  - type: textarea
    id: contact_communication
    attributes:
      label: Specify the vendor primary contact email or phone number
    validations:
      required: true

  - type: textarea
    id: address
    attributes:
      label: Specify the vendor headquarters address
    validations:
      required: true

  - type: textarea
    id: dateofassessment
    attributes:
      label: Specify the assessment date
    validations:
      required: true

  - type: textarea
    id: services
    attributes:
      label: List the services provided by the vendor
    validations:
      required: true

  - type: checkboxes
    attributes:
      label: Criticality
      description: Select which level of criticality for this assessment
      options:
      - label: High
      - label: Medium
      - label: Low
    validations:
      required: true

  - type: checkboxes
    attributes:
      label: Type(s) of data shared
      description: Select which types of data would be shared
      options:
      - label: PII
      - label: PCI
      - label: Other
    validations:
      required: true
