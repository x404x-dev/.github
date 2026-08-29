<div align="center">

# ⚙️ .github — GitHub Profile & Automation Config
Repository này chứa mã nguồn, workflow tự động hóa và tài nguyên cấu hình cho trang cá nhân GitHub của tôi.

</div>
<p align="center">
  <a href="https://github.com/x404x-dev"><img src="https://img.shields.io/badge/Xem_Trang_Cá_Nhân_(Profile)-181717?style=for-the-badge&logo=github&logoColor=white" alt="Visit Profile" /></a>
  <a href="./profile/README.md"><img src="https://img.shields.io/badge/Xem_File_Generated_README-2088FF?style=for-the-badge&logo=markdown&logoColor=white" alt="View Generated README" /></a>
</p>

---

### 📁 Cấu trúc Thư mục (Project Structure)

```text
.github/
├── .github/workflows/   # Các GitHub Actions chạy tự động
│   ├── snake.yml
│   └── update.yml
├── profile/             # Output folder (Do GitHub quy định để hiển thị bio)
│   └── README.md
└── src/                 # Source code & Templates gốc
    ├── icons/
    ├── snake/
    ├── README.md
    └── icons.json

```

---

### 🔄 Cách thức Hoạt động (How It Works)

1. **Source Template**: Toàn bộ nội dung gốc và cấu hình biến tùy chỉnh nằm tại `src/README.md`.
2. **Automated Pipeline**: Khi có thay đổi hoặc theo lịch trình, GitHub Actions (`update.yml` & `snake.yml`) sẽ kích hoạt.
3. **Build & Render**: Workflow tự động thay thế các biến, cập nhật dữ liệu mới nhất (snake animation, stats...) và xuất file kết quả ra `profile/README.md`.
4. **Publish**: GitHub sẽ tự động lấy file `profile/README.md` để hiển thị trực tiếp lên trang cá nhân.

---

> [!NOTE]
> Mọi thay đổi nội dung Bio vui lòng chỉnh sửa tại **`src/README.md`**, không sửa trực tiếp trong thư mục `profile/`.
