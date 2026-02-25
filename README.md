# Hello Git - Branching & Merging Practice

## 📌 Giới thiệu

Repository này dùng để thực hành các thao tác quan trọng trong Git:
- Tạo và quản lý branch
- Merge branch
- Xử lý merge conflict
- Quan sát commit graph
- Hiểu cơ chế hoạt động của HEAD, local branch và remote-tracking branch

---

## 🧩 Bài 1 – Feature Branch Workflow

### Mục tiêu
Hiểu quy trình làm việc cơ bản với feature branch.

### Thực hiện
- Tạo `main` với nhiều commit nền tảng
- Tạo branch `feature-a` từ `main`
- Thực hiện commit trên `feature-a`
- Merge `feature-a` vào `main`
- Quan sát merge commit trong commit graph

### Kiến thức đạt được
- Branch là con trỏ đến commit
- Merge tạo commit mới khi có lịch sử tách nhánh

---

## 🔀 Bài 2 – Multiple Parallel Branches

### Mục tiêu
Hiểu cách nhiều branch phát triển song song và cách merge tuần tự.

### Thực hiện
- Tạo 3 branch: `x`, `y`, `z` từ cùng một commit
- Commit riêng trên từng branch
- Merge lần lượt từng branch vào `main`
- Xử lý conflict nếu có
- Phân tích commit graph sau khi merge

### Kiến thức đạt được
- Merge conflict xảy ra khi nhiều branch chỉnh sửa cùng một vùng code
- Cách Git tạo merge commit khi tích hợp nhiều nhánh

---

## 🌳 Bài 3 – Develop Workflow Simulation

### Mục tiêu
Mô phỏng quy trình làm việc nhóm theo mô hình có nhánh `develop`.

### Thực hiện
- Tạo branch `develop` từ `main`
- Tạo các feature branch từ `develop`
- Merge feature → develop
- Merge develop → main
- Quan sát luồng phát triển nhiều tầng

### Kiến thức đạt được
- Workflow theo mô hình nhiều môi trường
- Tách biệt môi trường phát triển và môi trường ổn định

---

## 📊 Kiến thức tổng hợp

- `HEAD` là con trỏ đặc biệt trỏ tới branch hiện tại
- `main`, `develop`, `feature-*` là local branches
- `origin/main` là remote-tracking branch trong local
- `git fetch` chỉ cập nhật remote-tracking branch
- `git pull` = fetch + merge
- Conflict cần được giải quyết trước khi hoàn tất merge

---

## 🔍 Cách quan sát commit graph

```bash
git log --oneline --graph --all