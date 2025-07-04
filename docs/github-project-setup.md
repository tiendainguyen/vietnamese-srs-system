# 📋 GitHub Project Board Setup Guide

## 🎯 Tạo Kanban Board cho Sprint Management

### Bước 1: Tạo Project mới
1. Vào repository: https://github.com/tiendainguyen/vietnamese-srs-system
2. Click tab **"Projects"** ở menu trên
3. Click **"New project"**
4. Chọn **"Board"** template
5. Đặt tên: **"🇻🇳 Vietnamese SRS - Sprint Management"**
6. Mô tả: **"Kanban board for managing development sprints and tasks"**
7. Visibility: **Public** (hoặc Private tùy theo team)

### Bước 2: Cấu hình Columns
Tạo các columns sau (theo thứ tự):

1. **📝 Backlog**
   - Mô tả: Tasks chưa được assign hoặc chưa ready
   - Automation: None

2. **🔄 Ready**
   - Mô tả: Tasks ready để bắt đầu làm
   - Automation: None

3. **🏗️ In Progress**  
   - Mô tả: Tasks đang được develop
   - Automation: Auto-move when issue is assigned

4. **👀 In Review**
   - Mô tả: Tasks đang được code review
   - Automation: Auto-move when PR is opened

5. **✅ Done**
   - Mô tả: Tasks đã hoàn thành
   - Automation: Auto-move when issue is closed

### Bước 3: Add Issues vào Project

#### Automatic method (Recommended):
1. Trong Project settings, enable **Auto-add**
2. Set filter: `repo:tiendainguyen/vietnamese-srs-system`
3. Tất cả issues mới sẽ tự động được add vào Backlog

#### Manual method:
1. Click **"Add item"** trong project
2. Search và select issues muốn add:
   - #1 Sprint 1: Cơ sở hạ tầng (Epic)
   - #2 BE-1.1.1: Node.js/Express Server Setup
   - #3 BE-1.1.2: Docker Configuration  
   - #4 FE-1.1.1: React Application Setup
   - #5 BE-1.2.1: PostgreSQL & Prisma Setup
   - #6 BE-1.2.2: Core Database Schema Design
   - #7 BE-1.3.1: JWT Authentication System
   - #8 FE-1.3.1: Authentication UI Components

### Bước 4: Organize Sprint 1 Tasks

**Di chuyển các tasks vào columns phù hợp:**

#### 📝 Backlog:
- #1 Sprint 1: Cơ sở hạ tầng (Epic - for tracking)

#### 🔄 Ready (Ready to start):
- #2 BE-1.1.1: Node.js/Express Server Setup  
- #4 FE-1.1.1: React Application Setup

#### Remaining tasks đợi dependencies:
- #3 BE-1.1.2: Docker Configuration (after #2)
- #5 BE-1.2.1: PostgreSQL & Prisma Setup (after #3)
- #6 BE-1.2.2: Core Schema Design (after #5)  
- #7 BE-1.3.1: JWT Authentication (after #6)
- #8 FE-1.3.1: Authentication UI (after #7)

### Bước 5: Setup Custom Fields (Optional)

Add custom fields để track thêm info:

1. **Estimate** (Number field)
   - Unit: Days
   - Giá trị: 1, 2, 3 days

2. **Priority** (Single select)
   - Options: Critical, High, Medium, Low

3. **Sprint** (Single select)  
   - Options: Sprint 1, Sprint 2, Sprint 3, etc.

4. **Role** (Single select)
   - Options: Backend, Frontend, DevOps, Design

### Bước 6: Team Workflow

#### Khi bắt đầu task:
1. Assign issue cho developer
2. Move từ **Ready** → **In Progress**
3. Create branch từ main: `feature/issue-number-brief-description`

#### Khi hoàn thành development:
1. Create Pull Request
2. Move task từ **In Progress** → **In Review**  
3. Request review từ team members

#### Khi được approve:
1. Merge PR
2. Task tự động move vào **Done**
3. Close issue

### Bước 7: Sprint Tracking

#### Daily Standup sử dụng board:
- Review **In Progress** tasks
- Identify blockers
- Update progress

#### Sprint Review:
- Count completed tasks in **Done**
- Measure velocity (completed story points)
- Plan next sprint

### 🎯 Current Sprint 1 Status

**Ready to Start** (2 tasks):
- BE-1.1.1: Node.js/Express setup (2 days)
- FE-1.1.1: React application setup (1 day)

**Waiting Dependencies** (6 tasks):
- Remaining backend infrastructure
- Database setup
- Authentication system

**Total Sprint 1**: 8 tasks = 15 days estimate

### 📊 Success Metrics

Track these KPIs trong Project:
- **Sprint Velocity**: Tasks completed per sprint  
- **Cycle Time**: Time từ Ready → Done
- **Burndown**: Tasks remaining vs time
- **Blockers**: Issues stuck in review

### 🔧 Advanced Features

#### Automation Rules:
1. **Auto-assign to In Progress** khi issue được assign
2. **Auto-move to Review** khi PR được tạo
3. **Auto-close** khi PR được merge

#### Views:
1. **By Sprint**: Filter theo sprint number
2. **By Assignee**: Xem workload của từng người
3. **By Priority**: Focus vào critical tasks trước

---

## 🚀 Getting Started

1. **Project Owner**: Tạo project board theo guide trên
2. **Team Members**: 
   - Bookmark project URL
   - Pick tasks từ **Ready** column
   - Update progress daily
3. **Start Development**: Begin với tasks #2 và #4!

## 📞 Support

Nếu cần hỗ trợ setup project board:
- Check GitHub Projects documentation
- Ask team lead hoặc DevOps engineer
- Reference video tutorials trên GitHub

**Happy coding! 🇻🇳**