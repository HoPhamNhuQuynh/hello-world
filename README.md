# Hello Git - Branching & Merging Practice

## 📌 Mục tiêu
Thực hành các thao tác với Git:
- Tạo branch
- Commit trên từng branch
- Merge branch
- Xử lý conflict
- Quan sát commit graph

---

## 🧩 Bài 1 - Feature Branch Workflow

- Tạo `main` với 3 commit
- Tạo branch `feature-a`
- Commit trên `feature-a`
- Tạo Pull Request và merge vào `main`
- Quan sát merge commit trong graph

---

## 🔀 Bài 2 - Parallel Branches

- Tạo 3 branch: `x`, `y`, `z`
- Commit riêng trên từng branch
- Merge lần lượt vào `main`
- Xử lý conflict khi merge
- Quan sát commit graph phức tạp hơn

---

## 🌳 Bài 3 - Develop Workflow

- Tạo branch `develop` từ `main`
- Tạo các feature branch từ `develop`
- Merge feature → develop
- Merge develop → main
- Mô phỏng quy trình làm việc nhóm

---

## 📊 Kiến thức rút ra

- Branch là con trỏ đến commit
- `origin/main` là remote-tracking branch
- `git fetch` chỉ cập nhật remote-tracking branch
- `git pull` = fetch + merge
- Conflict xảy ra khi 2 branch sửa cùng một vùng code

---

## 🛠 Công cụ sử dụng

- Git
- GitHub
- PowerShell / Terminal

---

> Lab này giúp hiểu sâu về commit graph và cơ chế hoạt động của branch trong Git.