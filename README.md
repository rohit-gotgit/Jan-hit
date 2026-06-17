<div align="center">

# 🏛️ Janhit - Civic Engagement Platform 
**Empowering Communities Through Digital Democracy**

<br>

<img src="https://img.shields.io/badge/React-Frontend-61DAFB?logo=react&logoColor=white" />
<img src="https://img.shields.io/badge/Node.js-Backend-339933?logo=node.js&logoColor=white" />
<img src="https://img.shields.io/badge/MongoDB-Database-47A248?logo=mongodb&logoColor=white" />
<img src="https://img.shields.io/badge/Leaflet-Geospatial%20Mapping-199900" />
<img src="https://img.shields.io/badge/JWT-Secure%20Authentication-orange" />
<img src="https://img.shields.io/badge/Role--Based-Access%20Control-blueviolet" />

</div>

---

##  Overview

**Janhit** is a revolutionary civic engagement platform that bridges the gap between citizens and local government. Built with cutting-edge technology, it provides a seamless way for residents to report, track, and resolve community issues while enabling officials to manage and prioritize problems efficiently.

###  Mission
Transform local governance by creating a transparent, accountable, and participatory system where every citizen's voice matters.

---

##  Key Features

###  **Interactive Map-Based Reporting**
- **Pin-drop functionality** for precise issue location
- **Real-time geolocation** integration
- **Visual problem mapping** with categorized markers
- **Distance-based sorting** for local relevance

###  **Democratic Voting System**
- **Severity-based voting** (1-5 scale)
- **Community-driven prioritization**
- **Automatic vote counting** for issues with severity ≥3
- **Transparent rating system**

###  **Dual User Interface**
- **Citizen Dashboard**: Report issues, track progress, vote on problems
- **Official Dashboard**: Manage assignments, update status, resolve issues
- **Role-based access control** with JWT authentication

###  **Social Engagement**
- **Comment system** for community discussion
- **Real-time updates** on issue status
- **User interaction** and feedback loops
- **Issue categorization** (Road, Sewage, Garbage, etc.)

###  **Advanced Analytics**
- **Issue tracking** with status updates
- **Vote analytics** and community sentiment
- **Geographic problem clustering**
- **Performance metrics** for officials

---

##  Technology Stack

### Frontend
- **React 18** with TypeScript for type safety
- **Leaflet.js** for interactive mapping
- **Tailwind CSS** for modern, responsive design
- **React Router** for seamless navigation
- **Axios** for API communication
- **React Hot Toast** for user notifications

### Backend
- **Node.js** with Express.js framework
- **MongoDB** with Mongoose ODM
- **JWT Authentication** for secure access
- **RESTful API** architecture
- **Geospatial indexing** for location-based queries

### DevOps & Deployment
- **Vercel** for frontend hosting
- **Environment-based configuration**
- **CORS-enabled** for cross-origin requests
- **Production-ready** deployment setup

---

##  Live Demo

**Experience Janhit in action:** [https://janhit-flame.vercel.app/](https://janhit-flame.vercel.app/)

###  Demo Credentials
**Test the application with these demo credentials:**

| Role | Email | Password |
|------|-------|----------|
| Citizen | `random@gmail.com` | `12345` |
| Official | `random@gmail.com` | `12345` |

> **Note:** Use the same credentials for both citizen and official roles to explore different features of the platform.

---

##  Screenshots

###  Homepage
![Homepage](https://github.com/user-attachments/assets/c76bc122-98c4-4adf-9502-d47b2ee9e2b3)

###  Interactive Map
![Interactive Map](https://github.com/user-attachments/assets/2369af92-03aa-4c2b-9574-96d1a662fdf8)

###  User Dashboard
![User Dashboard](https://github.com/user-attachments/assets/fa27ddcd-0081-42f3-87b6-d2a924cd4e83)

###  Official Dashboard
![Official Dashboard](https://github.com/user-attachments/assets/be75a3d2-7060-40a0-9356-400a89583cdd)

###  Issue Management
![Issue Management](https://github.com/user-attachments/assets/bffd4cd4-d8e3-4efb-a6a4-57fd35022875)

---

##  Architecture

```
Janhit/
├── Client/                 # React Frontend
│   ├── src/
│   │   ├── components/    # Reusable UI components
│   │   ├── pages/        # Route components
│   │   ├── assets/       # Static assets
│   │   └── ApiUri.ts     # API configuration
│   └── public/           # Public assets
├── Server/                # Node.js Backend
│   ├── src/
│   │   ├── controllers/  # Business logic
│   │   ├── models/       # MongoDB schemas
│   │   ├── routes/       # API endpoints
│   │   ├── middlewares/  # Authentication & validation
│   │   └── db/          # Database connection
│   └── package.json
└── README.md
```

---

##  Quick Start

### Prerequisites
- **Node.js** (v16 or higher)
- **MongoDB** (local or Atlas)
- **npm** or **yarn**

### 1. Clone Repository
```bash
git clone https://github.com/Rachit-31/Janhit.git
cd Janhit
```

### 2. Backend Setup
```bash
cd Server
npm install
```

Create `.env` file:
```env
MONGODB_URI=your_mongodb_connection_string
ACCESS_TOKEN_SECRET=your_jwt_secret
REFRESH_TOKEN_SECRET=your_refresh_secret
ACCESS_TOKEN_EXPIRY=15m
REFRESH_TOKEN_EXPIRY=7d
CORS=*
PORT=8000
```

### 3. Frontend Setup
```bash
cd Client
npm install
```

### 4. Start Development Servers

**Backend:**
```bash
cd Server
npm run dev
```

**Frontend:**
```bash
cd Client
npm run dev
```

Visit `http://localhost:5173` to see the application!

---

## 🔧 API Endpoints

### Authentication
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `POST /api/auth/logout` - User logout

### Issues
- `GET /api/problems` - Get all issues
- `POST /api/problems` - Create new issue
- `PUT /api/problems/:id` - Update issue
- `DELETE /api/problems/:id` - Delete issue

### Voting & Comments
- `POST /api/votes` - Vote on issue
- `POST /api/comments` - Add comment
- `GET /api/comments/:problemId` - Get comments

### Officials
- `GET /api/officials` - Get officials
- `PUT /api/officials/assign` - Assign issue to official

---

##  Problem Statement

### The Challenge
Local communities face significant challenges in civic issue reporting:
- **Lack of centralized platforms** for issue reporting
- **Poor transparency** in issue resolution
- **No community involvement** in prioritization
- **Inefficient communication** between citizens and officials
- **Limited accountability** in local governance

### Our Solution
Janhit addresses these challenges by providing:
- **Centralized reporting system** with map integration
- **Transparent tracking** of issue resolution
- **Community-driven prioritization** through voting
- **Direct communication** between citizens and officials
- **Accountability mechanisms** for local governance

---

##  Key Benefits

### For Citizens
- **Easy reporting** with map-based interface
- **Real-time tracking** of issue status
- **Community participation** through voting
- **Transparent governance** with public updates

### For Officials
- **Efficient issue management** dashboard
- **Priority-based assignment** system
- **Performance tracking** and analytics
- **Streamlined communication** with citizens

### For Communities
- **Improved local infrastructure** through better reporting
- **Increased civic engagement** and participation
- **Data-driven decision making** for local governance
- **Enhanced transparency** in public services

---

##  Contributing

We welcome contributions! Please follow these steps:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/AmazingFeature`)
3. **Commit** your changes (`git commit -m 'Add some AmazingFeature'`)
4. **Push** to the branch (`git push origin feature/AmazingFeature`)
5. **Open** a Pull Request

### Development Guidelines
- Follow **TypeScript** best practices
- Maintain **consistent code style**
- Write **comprehensive tests**
- Update **documentation** for new features

---

##  Contact

**Project Lead:** Rohit Kumar  
**Email:** viciousdotro@gmail.com

**Team Members:**
- Rohit Kumar - Full Stack Developer
- Rachit - Backend Developer
- Additional team members

---

##  License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---

##  Acknowledgments

- **React Team** for the amazing frontend framework
- **Leaflet.js** for interactive mapping capabilities
- **MongoDB** for robust data storage
- **Vercel** for seamless deployment
- **Open Source Community** for inspiration and support

---


