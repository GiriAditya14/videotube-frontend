# Twideo Frontend - Modern Video Sharing Platform

<div align="center">

![React](https://img.shields.io/badge/React-v18.2.0-blue.svg)
![Vite](https://img.shields.io/badge/Vite-v5.2.0-purple.svg)
![Redux](https://img.shields.io/badge/Redux_Toolkit-v2.2.3-764ABC.svg)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-v3.4.3-38B2AC.svg)

A modern, responsive video-sharing platform frontend built with React, featuring real-time interactions, infinite scrolling, and a comprehensive content management system.

[Features](#-features) • [Tech Stack](#-tech-stack) • [Installation](#-installation) • [Live Demo](#-live-demo)

</div>

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [Pages & Components](#-pages--components)
- [State Management](#-state-management)
- [Installation](#-installation)
- [Environment Variables](#-environment-variables)
- [Deployment](#-deployment)
- [Performance Features](#-performance-features)

---

## 🎯 Overview

Twideo Frontend is a feature-rich, production-ready video-sharing platform interface that provides users with a seamless experience for uploading, watching, and interacting with video content. Built with modern React practices and optimized for performance, it offers a YouTube-like experience with additional blog/tweet functionality.

**Live Application:** [https://URL.vercel.app](https://URL.vercel.app)

---

## ✨ Features

### 🔐 Authentication & Authorization
- **User Registration** with avatar and cover image upload
- **Secure Login/Logout** with JWT token management
- **Protected Routes** using AuthLayout component
- **Persistent Sessions** with cookie-based authentication
- **Auto-redirect** for unauthorized access
- **Current User Context** maintained globally

### 🎥 Video Features
- **Video Upload** with drag-and-drop support
  - Real-time upload progress bar
  - File size validation
  - Format validation (MP4, AVI, MOV, WMV, MKV, FLV, WebM)
  - Thumbnail upload and preview
  - Title and description management
  - Publish/draft toggle
- **Video Player**
  - Custom HTML5 video player
  - Full-screen support
  - View count tracking
  - Video metadata display
  - Owner information with avatar
- **Video Management**
  - Edit video details and thumbnail
  - Delete videos
  - Toggle publish/unpublish status
  - Video statistics (views, likes, comments)
- **Video Discovery**
  - Home feed with infinite scrolling
  - Search functionality with filters
  - Sort by date, views, popularity
  - Channel-specific video listing
  - Lazy loading for performance
  - Skeleton loading states

### 💬 Comment System
- **Threaded Comments** on videos
- **Real-time Comment Count**
- **Add/Edit/Delete Comments**
- **Comment Likes** with toggle
- **User Information** display with avatars
- **Timestamp Display** (relative time)
- **Owner Verification** for edit/delete actions

### 👍 Like/Dislike System
- **Video Likes** with instant feedback
- **Comment Likes** for engagement
- **Tweet/Blog Likes** for written content
- **Like Count Display** in real-time
- **Visual Indication** of like status
- **Toggle Functionality** (like/unlike)

### 📱 Subscription System
- **Channel Subscription** with single click
- **Subscriber Count** display
- **Subscription Status** indication
- **Subscribed Channels Feed**
- **Channel Discovery**
- **Unsubscribe Functionality**

### 📝 Tweet/Blog Features
- **Rich Text Editor** for blog creation
- **Create/Edit/Delete Blogs**
- **User Blog Feed**
- **Global Blog Timeline**
- **Blog Cards** with preview
- **Like and Comment** on blogs
- **Author Information** display

### 📚 Playlist Management
- **Create Custom Playlists**
  - Name and description
  - Public/private toggle
- **Add/Remove Videos** from playlists
- **Playlist Cards** with video count
- **Playlist Feed Page**
- **Video Thumbnails** preview
- **Edit Playlist Details**
- **Delete Playlists**
- **Channel Playlists** view

### 👤 User Profile & Channel
- **Channel Profile Page**
  - User information (avatar, cover, bio)
  - Video count and subscriber count
  - Channel videos grid
  - Channel playlists
  - Channel blogs/tweets
- **User Settings**
  - Update profile information
  - Change avatar and cover image
  - Update password
  - Account preferences
- **Watch History**
  - Chronological history tracking
  - Remove individual videos
  - Clear entire history
  - Timestamp display

### 📊 Creator Dashboard
- **Channel Statistics**
  - Total views
  - Total subscribers
  - Total videos
  - Total likes
- **Video Management Panel**
  - All uploaded videos
  - Quick edit access
  - Publish/unpublish toggle
  - Delete functionality
  - Performance metrics per video
- **Playlist Management**
  - All playlists overview
  - Quick access to edit
  - Video count per playlist

### 🎨 UI/UX Features
- **Fully Responsive Design**
  - Mobile-first approach
  - Tablet optimization
  - Desktop enhancements
  - Adaptive layouts
- **Dark/Light Theme Toggle**
  - System preference detection
  - Manual theme switching
  - Persistent theme storage
  - Smooth transitions
- **Infinite Scrolling**
  - Automatic content loading
  - Scroll position maintenance
  - Loading indicators
  - End-of-content detection
- **Progress Indicators**
  - Upload progress bar
  - Loading spinners
  - Skeleton screens
  - State feedback
- **Toast Notifications**
  - Success messages
  - Error alerts
  - Info notifications
  - Auto-dismiss
  - Position control
- **Modal Dialogs**
  - Confirmation dialogs
  - Form modals
  - Image preview
  - Overlay management
- **Dropdown Menus**
  - User menu
  - Video options
  - Filter selections
  - Accessible design
- **Navigation**
  - Sticky header
  - Sidebar navigation
  - Mobile hamburger menu
  - Active route highlighting
  - Breadcrumbs

### 🔍 Search & Discovery
- **Global Search**
  - Video search
  - Channel search
  - Real-time results
  - Search history
- **Filters & Sorting**
  - Sort by date
  - Sort by views
  - Sort by popularity
  - Filter by user
- **Recommendations**
  - Related videos
  - Suggested channels

### ⚡ Performance Optimizations
- **Code Splitting** with React.lazy
- **Lazy Loading** for images and videos
- **Debounced Search** for better UX
- **Memoization** with React.memo
- **Virtual Scrolling** for large lists
- **Image Optimization**
- **Bundle Size Optimization**
- **Fast Refresh** with Vite HMR

---

## 🚀 Tech Stack

### Core Framework
- **React 18.2.0** - UI library with hooks
- **Vite 5.2.0** - Next-generation build tool
- **React Router DOM 6.22.3** - Client-side routing

### State Management
- **Redux Toolkit 2.2.3** - State management
- **React Redux 9.1.0** - React bindings for Redux

### Styling
- **TailwindCSS 3.4.3** - Utility-first CSS framework
- **PostCSS 8.4.38** - CSS processing
- **Autoprefixer 10.4.19** - Vendor prefix automation

### Form Handling
- **React Hook Form 7.51.3** - Performant form management

### HTTP Client
- **Axios 1.6.8** - Promise-based HTTP client

### UI Components & Icons
- **FontAwesome 6.5.2** - Icon library
  - Solid icons
  - Regular icons
  - Brand icons
- **React FontAwesome 0.2.0** - React wrapper

### Notifications
- **React Toastify 10.0.5** - Toast notifications

### Loading States
- **React Spinners 0.13.8** - Loading indicators

### Cookie Management
- **React Cookie 7.1.4** - Cookie handling

### Development Tools
- **ESLint 8.57.0** - Code linting
- **Prettier** - Code formatting
- **Vite Plugin React 4.2.1** - Fast refresh

---

## 📁 Project Structure

```
src/
├── components/              # Reusable UI components
│   ├── Alert.jsx           # Alert/notification component
│   ├── Appearance.jsx      # Theme settings
│   ├── AuthLayout.jsx      # Authentication wrapper
│   ├── Dropdown.jsx        # Dropdown menu
│   ├── Input.jsx           # Form input component
│   ├── Layout.jsx          # Main layout wrapper
│   ├── LikeBtn.jsx         # Like button component
│   ├── Loader.jsx          # Loading spinner
│   ├── Logo.jsx            # App logo
│   ├── Modal.jsx           # Modal dialog
│   ├── Progressbar.jsx     # Progress indicator
│   ├── SubscribeBtn.jsx    # Subscribe button
│   ├── Blog/               # Blog-related components
│   │   ├── BlogCard.jsx
│   │   ├── BlogEditor.jsx
│   │   └── ChannelBlog.jsx
│   ├── Comment/            # Comment components
│   │   └── [Comment components]
│   ├── Dashboard/          # Dashboard components
│   │   ├── DashboardPlaylist.jsx
│   │   └── DashboardVideo.jsx
│   ├── Navigation/         # Navigation components
│   │   └── [Nav components]
│   ├── Playlist/           # Playlist components
│   │   └── [Playlist components]
│   ├── Setting/            # Settings components
│   │   └── [Settings components]
│   └── Video/              # Video-related components
│       ├── ChannelVideos.jsx
│       ├── EditVideo.jsx
│       ├── UploadVideo.jsx
│       ├── VideoCard.jsx
│       ├── VideoContainer.jsx
│       ├── VideoPageSkeleton.jsx
│       ├── VideoPlayer.jsx
│       └── VideoSkeleton.jsx
├── pages/                  # Page components
│   ├── Blog.jsx            # Blog/tweets page
│   ├── Dashboard.jsx       # Creator dashboard
│   ├── Home.jsx            # Home feed
│   ├── Login.jsx           # Login page
│   ├── Playlist.jsx        # User playlists
│   ├── PlaylistFeed.jsx    # Playlist details
│   ├── Profile.jsx         # User/channel profile
│   ├── SearchPage.jsx      # Search results
│   ├── Setting.jsx         # User settings
│   ├── Signup.jsx          # Registration page
│   ├── Video.jsx           # Video player page
│   └── WatchHistory.jsx    # Watch history
├── services/               # API service layer
│   ├── conf.js             # Axios configuration
│   ├── comment.service.js  # Comment APIs
│   ├── dashboard.service.js # Dashboard APIs
│   ├── like.service.js     # Like APIs
│   ├── playlist.service.js # Playlist APIs
│   ├── subscription.service.js # Subscription APIs
│   ├── tweet.service.js    # Tweet/blog APIs
│   ├── user.service.js     # User APIs
│   └── video.service.js    # Video APIs
├── store/                  # Redux store
│   ├── store.js            # Store configuration
│   ├── navbarSlice.js      # Navbar state
│   ├── playlistSlice.js    # Playlist state
│   ├── tweetSlice.js       # Tweet state
│   ├── userSlice.js        # User state
│   └── videoSlice.js       # Video state
├── context/                # React Context
│   └── Theme/              # Theme context
├── hooks/                  # Custom hooks
│   └── useErrorMessage.js  # Error handling hook
├── utils/                  # Utility functions
│   ├── formatVideoDuration.js
│   ├── formatViews.js
│   └── [other utilities]
├── assets/                 # Static assets
├── App.jsx                 # Root component
├── main.jsx                # Entry point
├── App.css                 # Global styles
└── index.css               # Base styles
```

---

## 📄 Pages & Components

### Pages

#### **Home (`Home.jsx`)**
- Video feed with infinite scrolling
- Featured videos
- Skeleton loading states
- Search integration
- Sort and filter options

#### **Video (`Video.jsx`)**
- Video player with controls
- Video metadata (title, views, date)
- Like/dislike buttons
- Subscribe button
- Comment section
- Related videos sidebar

#### **Profile (`Profile.jsx`)**
- User/channel information
- Avatar and cover image
- Subscriber count
- Tabs: Videos, Playlists, Tweets
- Subscribe button (if not own channel)

#### **Dashboard (`Dashboard.jsx`)**
- Channel statistics
- Video management table
- Playlist management
- Quick actions
- Performance metrics

#### **Playlist (`Playlist.jsx`)**
- User's playlists grid
- Create new playlist
- Playlist cards with video count
- Edit/delete options

#### **PlaylistFeed (`PlaylistFeed.jsx`)**
- Playlist details
- Video list
- Play all functionality
- Add/remove videos
- Playlist metadata

#### **Blog (`Blog.jsx`)**
- Tweet/blog feed
- Create new blog
- Like and comment
- User blog filtering
- Pagination

#### **SearchPage (`SearchPage.jsx`)**
- Search results
- Filter options
- Sort functionality
- Video/channel tabs
- Empty state handling

#### **WatchHistory (`WatchHistory.jsx`)**
- Chronological history
- Remove individual items
- Clear all history
- Video cards with metadata

#### **Setting (`Setting.jsx`)**
- Profile settings
- Password change
- Avatar/cover upload
- Theme preferences
- Account management

#### **Login/Signup (`Login.jsx`, `Signup.jsx`)**
- Form validation
- Error handling
- Redirect logic
- Social login placeholders
- Responsive design

### Key Components

#### **Video Components**
- `VideoCard` - Video thumbnail with metadata
- `VideoPlayer` - Custom video player
- `VideoContainer` - Video grid wrapper
- `VideoSkeleton` - Loading placeholder
- `UploadVideo` - Upload form with progress
- `EditVideo` - Edit video details
- `ChannelVideos` - Channel video grid

#### **Blog Components**
- `BlogCard` - Blog post card
- `BlogEditor` - Rich text editor
- `ChannelBlog` - Channel blog feed

#### **Dashboard Components**
- `DashboardVideo` - Video management table
- `DashboardPlaylist` - Playlist management

#### **Shared Components**
- `Layout` - Main app layout
- `AuthLayout` - Protected route wrapper
- `Input` - Styled form input
- `Modal` - Reusable modal dialog
- `Dropdown` - Dropdown menu
- `LikeBtn` - Like button with state
- `SubscribeBtn` - Subscribe button
- `Loader` - Loading spinner
- `Progressbar` - Upload progress
- `Alert` - Alert notifications

---

## 🗃️ State Management

### Redux Slices

#### **User Slice (`userSlice.js`)**
```javascript
{
  user: null,           // Current user data
  status: 'idle',       // Loading status
  isAuthenticated: false
}
```

#### **Video Slice (`videoSlice.js`)**
```javascript
{
  videos: [],           // Video list
  currentVideo: null,   // Currently playing video
  loading: false,
  error: null,
  hasMore: true,        // Infinite scroll flag
  page: 1
}
```

#### **Playlist Slice (`playlistSlice.js`)**
```javascript
{
  playlists: [],
  currentPlaylist: null,
  loading: false
}
```

#### **Tweet Slice (`tweetSlice.js`)**
```javascript
{
  tweets: [],
  loading: false,
  hasMore: true
}
```

#### **Navbar Slice (`navbarSlice.js`)**
```javascript
{
  isOpen: false,        // Mobile menu state
  activeTab: 'home'
}
```

---

## 🛠️ Installation

### Prerequisites
- Node.js (v18 or higher)
- npm or yarn
- Git

### Local Development Setup

1. **Clone the repository**
   ```bash
   git clone <your-repository-url>
   cd "Twideo frontend"
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure environment variables**
   
   Create a `.env` file in the root directory:
   ```bash
   cp .env.sample .env
   ```

4. **Start development server**
   ```bash
   npm run dev
   ```

5. **Build for production**
   ```bash
   npm run build
   ```

6. **Preview production build**
   ```bash
   npm run preview
   ```

The application will be available at `http://localhost:5173`

---

## 🔐 Environment Variables

Create a `.env` file with the following variables:

```env
# Backend API URL
VITE_SERVER_URI=https://your-backend-api.onrender.com

# Video Upload Limitations
VITE_LIMIT_VIDEO_UPLOAD_SIZE=true
VITE_LIMIT_VIDEO_UPLOAD_SIZE_VALUE=52428800

# Testing Configuration (Optional)
VITE_TEST_MODE=false
VITE_TEST_USERNAME=tester_username
VITE_TEST_PASSWORD=tester_password
```

### Variable Descriptions

- `VITE_SERVER_URI`: Backend API base URL
- `VITE_LIMIT_VIDEO_UPLOAD_SIZE`: Enable/disable size limit (true/false)
- `VITE_LIMIT_VIDEO_UPLOAD_SIZE_VALUE`: Maximum upload size in bytes (default: 50MB)
- `VITE_TEST_MODE`: Enable test mode with pre-filled credentials
- `VITE_TEST_USERNAME`: Test account username
- `VITE_TEST_PASSWORD`: Test account password

---

## ⚡ Performance Features

### Implemented Optimizations

1. **Code Splitting**
   - Route-based splitting
   - Component lazy loading
   - Dynamic imports

2. **Image Optimization**
   - Lazy loading images
   - Cloudinary CDN delivery
   - Responsive images
   - Thumbnail optimization

3. **Infinite Scrolling**
   - Load on scroll
   - Virtual scrolling
   - Pagination
   - Skeleton screens

4. **Caching Strategy**
   - API response caching
   - Redux state persistence
   - Browser storage utilization

5. **Bundle Optimization**
   - Tree shaking
   - Minification
   - Compression
   - Vite build optimization

6. **Performance Metrics**
   - Fast page loads
   - Smooth animations
   - Optimized re-renders
   - Debounced inputs

---

## 🎨 Design Features

### Responsive Design
- **Mobile First** approach
- Breakpoints: 640px, 768px, 1024px, 1280px
- Flexible grid layouts
- Touch-friendly interactions

### Dark/Light Theme
- System preference detection
- Manual toggle
- Persistent storage
- Smooth transitions
- Accessible contrast ratios

### Accessibility
- Semantic HTML
- ARIA labels
- Keyboard navigation
- Screen reader support
- Focus management

---

## 🧪 Testing

```bash
# Run linter
npm run lint

# Build test
npm run build

# Preview build
npm run preview
```

---

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

---

## 🔄 API Integration

### Services Layer

All API calls are centralized in the `services/` directory:

- **conf.js**: Axios instance configuration
- **user.service.js**: User authentication and profile APIs
- **video.service.js**: Video CRUD operations
- **comment.service.js**: Comment management
- **like.service.js**: Like/unlike operations
- **subscription.service.js**: Subscription management
- **playlist.service.js**: Playlist operations
- **tweet.service.js**: Blog/tweet APIs
- **dashboard.service.js**: Analytics and statistics

### Axios Configuration
```javascript
{
  baseURL: `${VITE_SERVER_URI}/api/v1`,
  withCredentials: true,
  headers: {
    'Accept': 'application/json',
    'Content-Type': 'application/json'
  }
}
```

---

## 📊 Features Comparison

| Feature | Implementation | Status |
|---------|---------------|--------|
| User Authentication | JWT + Cookies | ✅ |
| Video Upload | Cloudinary | ✅ |
| Video Player | Custom HTML5 | ✅ |
| Comments | Nested | ✅ |
| Likes | Toggle | ✅ |
| Subscriptions | Real-time | ✅ |
| Playlists | CRUD | ✅ |
| Blogs/Tweets | Full featured | ✅ |
| Search | With filters | ✅ |
| Dashboard | Analytics | ✅ |
| Dark Mode | Toggle | ✅ |
| Responsive | All devices | ✅ |
| Infinite Scroll | Auto-load | ✅ |
| Watch History | Tracked | ✅ |

---

## 🤝 Contributing

This is a portfolio project. For suggestions or improvements, please open an issue or submit a pull request.

---

## 📝 License

ISC

---

## 👨‍💻 Author

**Aditya Giri**

Built as a full-stack portfolio project demonstrating expertise in:
- Modern React development
- State management with Redux Toolkit
- Responsive UI design with TailwindCSS
- API integration
- Performance optimization
- Production deployment

---

**⭐ If you found this project helpful, please give it a star!**

---

## 🚀 Quick Start Guide

```bash
# Clone repository
git clone <your-repo-url>
cd "Twideo frontend"

# Install dependencies
npm install

# Setup environment
cp .env.sample .env
# Edit .env with your backend URL

# Start development
npm run dev

# Build for production
npm run build

# Deploy to Vercel
vercel --prod
```

**Happy Coding! 🎉**