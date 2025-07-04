# 🇻🇳 Vietnamese SRS System
## Hệ thống Lặp lại Cách quãng cho Tiếng Việt

> Một nền tảng học tiếng Việt hiện đại sử dụng thuật toán Spaced Repetition System (SRS) được tối ưu hóa đặc biệt cho tiếng Việt.

## 🌟 Tổng quan

Hệ thống SRS tiếng Việt là một ứng dụng web giúp người học tiếng Việt ghi nhớ từ vựng và ngữ pháp một cách hiệu quả thông qua việc lặp lại có kế hoạch. Được thiết kế với những tính năng đặc biệt dành riêng cho tiếng Việt.

## ✨ Tính năng chính

### 🎯 Thuật toán SRS Tối ưu
- **SM-2 Algorithm** được cải tiến cho tiếng Việt
- Tính toán khoảng cách ôn tập dựa trên độ khó thanh điệu
- Điều chỉnh thông minh theo hiệu suất học tập

### 🇻🇳 Xử lý Tiếng Việt Chuyên sâu
- **Hỗ trợ Unicode đầy đủ** cho dấu thanh điệu
- **Phân tích 6 thanh điệu** cơ bản của tiếng Việt
- **Tách từ thông minh** (không khoảng trắng tự nhiên)
- **Phiên âm IPA/SAMPA** tự động

### 📚 Quản lý Thẻ học Thông minh
- Tạo thẻ với **audio và hình ảnh**
- **Tags và phân loại** theo chủ đề
- **Tích hợp từ điển** tiếng Việt
- **Ngữ cảnh văn hóa** và thành ngữ

### 📊 Analytics & Báo cáo
- **Theo dõi tiến độ** chi tiết
- **Thống kê hiệu suất** học tập
- **Biểu đồ trực quan** và insights
- **Xuất báo cáo** PDF/CSV

## 🏗️ Kiến trúc Hệ thống

```
vietnamese-srs-system/
├── backend/                 # Node.js + Express + TypeScript
│   ├── src/
│   │   ├── routes/          # API endpoints
│   │   ├── models/          # Database models (Prisma)
│   │   ├── services/        # Business logic
│   │   ├── utils/           # Vietnamese text processing
│   │   └── algorithms/      # SRS algorithms
│   ├── Dockerfile
│   └── docker-compose.yml
├── frontend/                # React + TypeScript + Tailwind
│   ├── src/
│   │   ├── components/      # Reusable components
│   │   ├── pages/           # Page components
│   │   ├── hooks/           # Custom React hooks
│   │   └── utils/           # Frontend utilities
│   └── Dockerfile
├── docs/                    # Documentation
└── scripts/                 # Deployment & utilities
```

## 🛠️ Tech Stack

### Backend
- **Runtime**: Node.js + Express.js
- **Language**: TypeScript
- **Database**: PostgreSQL + Prisma ORM
- **Cache**: Redis
- **Auth**: JWT tokens
- **Validation**: Zod/Joi

### Frontend
- **Framework**: React 18 + TypeScript
- **Styling**: Tailwind CSS
- **Routing**: React Router v6
- **State**: Context API + React Query
- **Charts**: Recharts/Chart.js

### DevOps
- **Containerization**: Docker + Docker Compose
- **CI/CD**: GitHub Actions
- **Monitoring**: Winston Logger
- **Testing**: Jest + React Testing Library

## 🚀 Quick Start

### Prerequisites
- Node.js 18+
- Docker & Docker Compose
- PostgreSQL 15+

### Development Setup

1. **Clone repository**
```bash
git clone https://github.com/tiendainguyen/vietnamese-srs-system.git
cd vietnamese-srs-system
```

2. **Backend setup**
```bash
cd backend
npm install
cp .env.example .env
# Cấu hình database trong .env
npm run dev
```

3. **Frontend setup**
```bash
cd frontend
npm install
npm start
```

4. **Docker setup (Recommended)**
```bash
docker-compose up -d
```

## 📋 Sprint Planning

Dự án được chia thành 8 sprint trong 4-6 tháng:

### 🏗️ Sprint 1: Cơ sở hạ tầng (2 tuần)
- [x] Setup Node.js/Express backend
- [x] React frontend initialization
- [x] Docker configuration
- [x] Database design
- [x] Authentication system

### 🇻🇳 Sprint 2: Xử lý Tiếng Việt (2 tuần)
- [ ] Unicode & tone processing
- [ ] Word segmentation
- [ ] Phonetic analysis (IPA/SAMPA)

### 🧮 Sprint 3: SRS Algorithm (2 tuần)
- [ ] SM-2 algorithm implementation
- [ ] Vietnamese-specific adaptations
- [ ] Review scheduling engine

### 📚 Sprint 4: Card Management (2 tuần)
- [ ] CRUD operations for cards
- [ ] Media upload (audio/images)
- [ ] Tagging system

### 🎨 Sprint 5: User Interface (3 tuần)
- [ ] Study session interface
- [ ] Dashboard & analytics
- [ ] Settings & preferences

### 📖 Sprint 6: Dictionary Integration (2 tuần)
- [ ] Lạc Việt API integration
- [ ] Auto card generation
- [ ] Cultural context suggestions

### 📊 Sprint 7: Analytics & Reporting (2 tuần)
- [ ] Learning progress tracking
- [ ] Performance analytics
- [ ] Export functionality

### 🔒 Sprint 8: Optimization & Security (2 tuần)
- [ ] Performance optimization
- [ ] Security hardening
- [ ] Production deployment

## 📚 Documentation

- [📋 Project Stories & Tasks](https://www.notion.so/Ph-n-chia-Story-H-th-ng-SRS-Ti-ng-Vi-t-2260b0210d8781b3a052e0cbcd577778)
- [🇻🇳 Vietnamese SRS System Docs](https://www.notion.so/H-th-ng-L-p-l-i-C-ch-qu-ng-Spaced-Repetition-System-Ti-ng-Vi-t-2260b0210d87802bad7df231fc7fa7f7)
- [🔧 API Documentation](./docs/api.md) (Coming soon)
- [🎨 UI/UX Design](./docs/design.md) (Coming soon)

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📊 Project Status

### Current Sprint: Sprint 1 - Infrastructure Foundation
**Progress**: 🟡 In Progress (0/13 tasks completed)

**Active Issues**:
- [#2 BE-1.1.1: Node.js/Express Server Setup](https://github.com/tiendainguyen/vietnamese-srs-system/issues/2)
- [#3 BE-1.1.2: Docker Configuration](https://github.com/tiendainguyen/vietnamese-srs-system/issues/3)
- [#4 FE-1.1.1: React Application Setup](https://github.com/tiendainguyen/vietnamese-srs-system/issues/4)

**Next Milestones**:
- Complete infrastructure setup
- Begin Vietnamese text processing features
- Implement core SRS algorithm

## 🏷️ License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Team

- **Backend Developer**: TBD
- **Frontend Developer**: TBD  
- **Full-stack Developer**: TBD
- **DevOps Engineer**: TBD

## 📞 Contact

- **Project Lead**: [Tiên Đại Nguyễn](https://github.com/tiendainguyen)
- **Email**: [your-email@example.com]
- **Notion Workspace**: [Vietnamese SRS Documentation](https://www.notion.so/Ph-n-chia-Story-H-th-ng-SRS-Ti-ng-Vi-t-2260b0210d8781b3a052e0cbcd577778)

---

⭐ **Star this repository** if you find it useful for learning Vietnamese!

🇻🇳 **Chúc bạn học tiếng Việt vui vẻ và hiệu quả!**