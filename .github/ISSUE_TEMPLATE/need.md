name: 🧩 Business Need
description: Nhu cầu nghiệp vụ cấp cao (Needs)
title: "[NEED-XX] "
labels: ["need"]
assignees: []

body:

* type: dropdown
  id: stakeholder
  attributes:
  label: Stakeholder
  options:
  - High
  - Medium
  - Low
  validations:
  required: true

* type: dropdown
  id: priority
  attributes:
  label: Priority
  options:
  - High
  - Medium
  - Low
  validations:
  required: true

* type: dropdown
  id: origin
  attributes:
  label: Origin
  options:
  - Khách hàng
  - Phòng Kho vận
  - Ban Lãnh đạo
  - Admin
  - Marketing
  - CSKH
  - CSKH / Ban LD
  validations:
  required: true
