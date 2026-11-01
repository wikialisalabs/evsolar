# ☀️ Smart Solar App & Admin Panel — Community Design System

> Hệ thống thiết kế cốt lõi (Community Design System) và bộ UI Kit cho ứng dụng Năng lượng Mặt trời Thông minh & Bảng Điều khiển Quản trị (Admin Panel).

![Figma Link](https://img.shields.io/badge/Figma-Design%20Kit-F24E1E?logo=figma&logoColor=white)
![Astro](https://img.shields.io/badge/Astro-7.x%20SSG-FF5D01?logo=astro&logoColor=white)
![Icons](https://img.shields.io/badge/Icons-5130%2B%20Outline-49DBC8)
![Components](https://img.shields.io/badge/Components-201%20Items-BEFF6C?labelColor=black)

---

## 📌 Sơ Đồ Kiến Trúc Hệ Thống

Xem tài liệu chi tiết đầy đủ tại: [ARCHITECTURE.md](file:///d:/solar/ARCHITECTURE.md)

```mermaid
graph TD
    subgraph UI_Layer ["🎨 UI Layer - Community Design System"]
        direction TB
        
        subgraph Design_Tokens ["1. Design Tokens (3 Lớp)"]
            Primitive["Primitive Tokens"] --> Semantic["Semantic Tokens"]
            Semantic --> Component_Tokens["Component Tokens"]
            Component_Tokens --> CSS_Vars["CSS Custom Properties"]
        end

        subgraph Style_Assets ["2. Tài Nguyên Thiết Kế & Colors"]
            Icons["5130+ Icon SVG<br/>Outline Style"]
            Colors["7 Brand Colors<br/>Teal #49DBC8 | Green #BEFF6C | Orange #FC7339<br/>Pink #FD9FDD | Purple #AF96FB | Yellow #FFF172 | Grey #EFEFEF"]
        end

        subgraph UI_Components ["3. 201 Components"]
            C1["Button & Badge & Input"]
            C2["Toggle & Card & Navbar"]
            C3["Avatar & Chart & More..."]
        end

        subgraph Previews ["4. 126 Trang Preview (Astro 7.x)"]
            P1["Dashboard & Crypto"]
            P2["Payment & Wallet"]
            P3["Auth & Invoice & Tracking & Maps"]
        end

        Design_Tokens --> UI_Components
        Style_Assets --> UI_Components
        UI_Components --> Previews
    end

    subgraph Core_Workspace ["📁 Cấu Trúc Workspace"]
        W_Docs["/docs (Token Explorer, Icon Search)"]
        W_Docs2["/docs2 (Thử nghiệm)"]
        W_Preview["/preview (126 trang Astro SSG)"]
        W_Page["/page (Landing page UI Kit)"]
    end

    UI_Layer --> Core_Workspace
```

---

## ⚡ Bắt Đầu Nhanh

### 1. Môi Trường Xem Trước 126 Màn Hình (`/preview`)

```bash
cd preview
pnpm install
pnpm dev
# Truy cập tại: http://localhost:4321
```

### 2. Trang Tra Cứu Token & Icon Thư Viện (`/docs`)

```bash
cd docs
npm install
npm run dev
# Truy cập tại: http://localhost:3000
```

---

## 🎨 Bản Vẽ Thiết Kế Figma

- **Figma File**: [nlpgroup — Smart Solar App - Admin Panel - UI Kit](https://embed.figma.com/design/eq0EA9dRSWfS2ivuFohJdg/nlpgroup--Smart-Solar-App---Admin-Panel---UI-Kit?embed-host=share)
