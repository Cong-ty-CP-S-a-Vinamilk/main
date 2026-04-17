name: "🧩 Business Need"
description: "Nhu cầu nghiệp vụ cấp cao (Needs) từ các Stakeholder"
title: "[NEED-XX] "
labels:
  - need
assignees: []

body:
  - type: input
    id: need_id
    attributes:
      label: Need ID
      description: "Mã số định danh cho Need (từ file Excel)"
      placeholder: "STRQ-01"
    validations:
      required: true

  - type: dropdown
    id: stakeholder
    attributes:
      label: Stakeholder nguồn gốc
      description: "Bên liên quan đưa ra yêu cầu"
      options:
        - Khách hàng (Customer)
        - Ban Lãnh đạo Vinamilk
        - Phòng Marketing Vinamilk
        - Phòng Kho vận (Logistics)
        - Bộ phận CSKH (Customer Service)
        - Quản trị viên (Admin)
    validations:
      required: true

  - type: dropdown
    id: collection_method
    attributes:
      label: Kỹ thuật thu thập yêu cầu
      options:
        - Bảng câu hỏi điều tra
        - Hội thảo
        - Phỏng vấn
        - Thẻ sự kiện
        - Phân tích tài liệu
        - Phân tích dữ liệu
        - Hội thảo chiến lược
        - Hội thảo chiến lược AI
    validations:
      required: true

  - type: textarea
    id: description
    attributes:
      label: Mô tả Need
      description: "Yêu cầu cụ thể từ Stakeholder"
      placeholder: "Khách hàng muốn tìm kiếm và xem thông tin sản phẩm sữa Vinamilk trên website một cách nhanh chóng."
    validations:
      required: true

  - type: dropdown
    id: priority
    attributes:
      label: Stakeholder Priority
      options:
        - H (High - Cao)
        - M (Medium - Trung bình)
        - L (Low - Thấp)
    validations:
      required: true

  - type: input
    id: origin
    attributes:
      label: Origin
      description: "Nguồn gốc yêu cầu"
      placeholder: "Khách hàng"

  - type: textarea
    id: related_features
    attributes:
      label: FEAT liên quan
      description: "Các Feature đáp ứng Need này"
      placeholder: "FEAT1, FEAT2"

  - type: textarea
    id: related_uc
    attributes:
      label: USE CASE liên quan
      description: "Các Use Case liên quan"
      placeholder: "UC-02"

  - type: textarea
    id: related_supl
    attributes:
      label: SUPL liên quan
      description: "Các Supplementary Requirements liên quan"
      placeholder: "SUP-01, SUP-04"
