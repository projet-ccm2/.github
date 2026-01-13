# StreamQuest - Interactive and Gamified Twitch Extension

## 🌍 Languages / Langues
- 🇫🇷 [Français](README.fr.md)
- 🇬🇧 **English** (current)

---

## 🎯 Project Overview

This project presents the development of an **interactive and gamified Twitch extension** that introduces an achievement/success system for viewers, aiming to increase engagement and loyalty within streamer communities.

## 🚀 Core Concept

### Gamification System
- **Unlockable achievements** based on viewer actions:
  - Watch time
  - Channel points spent
  - Specific interactions (e.g., saying "hello" in chat)
  - Hidden achievements to discover
- **Viewer leaderboard** displayable on the application
- **Exclusive badges** for the most invested viewers

### Achievement Creation
- **Simple mode**: easy creation for streamers
- **Advanced mode**: developer tools for complex achievements
- **Community suggestions** to enrich the catalog

## 🛠️ Additional Features

### 🌐 Multi-Platform
- **Twitch Extension** (main interface)
- **Web/mobile interface** for configuration and tracking
- **Discord Bot** connected (notifications, reminders)

### 📚 Public Library
- **Reusable achievements** between streamers
- **Public API** for external developers
- **Integration** with third-party applications

### 🤖 Artificial Intelligence
- Automatic generation of achievement titles/descriptions
- Relevant achievement suggestions based on the channel
- Message analysis for personalized suggestions

## 💻 Technologies and Skills Mobilized

### Cloud Computing
- **Google Cloud Platform (GCP)** for deployment
- **Cloud Run** for serverless microservices orchestration
- CI/CD, monitoring, automatic scalability

### Frontend Development
- **React** for web application
- **Capacitor** for mobile web app (iOS and Android)
- Multi-platform experience (Twitch + Mobile + Discord)

### Artificial Intelligence
- Automatic achievement generation
- Viewer behavioral analysis

### Programming & API
- **TypeScript** for reliability and maintainability
- Integration with **Twitch API**

## 🎮 Usage Examples

### Concrete Cases
- **Streamer A**: "Morning Loyal" achievement → say "hello" 3 consecutive days
- **Streamer B**: Hidden "Big Spender" achievement → spend 5000 channel points
- **Viewer**: "100 hours watched" badge in public leaderboard
- **Discord Bot**: "GG @User123, you just unlocked the *Absolute Fan* achievement!"

## 🎯 Motivations

- **Innovative** project close to our interests
- Valuing **gamification** as an engagement lever
- Demonstrating technical skills (Cloud + Mobile + API + AI)
- Real adoption potential by the streaming community

## 🏗️ Project Architecture

### Architecture Diagram

![Architecture Diagram](../docs/architecture-old.png)

*Add your architecture diagram in the `docs/` folder with the name `architecture.png`*

### Project Components & Progress

The **StreamQuest** project is structured in microservices deployed on **Google Cloud Platform** with **Cloud Run**:

#### Overall Status
![Issues](https://img.shields.io/github/issues/projet-ccm2/achievement-management)
![Pull Requests](https://img.shields.io/github/issues-pr/projet-ccm2/achievement-management)
![Last Commit](https://img.shields.io/github/last-commit/projet-ccm2/achievement-management)

#### 🔗 Core Services
| Service | Description | Issues | PRs | Status |
|---------|-------------|--------|-----|--------|
| [twitch-event-listener](https://github.com/projet-ccm2/twitch-event-listener) | *Listens to real-time Twitch events* (chat messages, subscriptions, donations) | ![Issues](https://img.shields.io/github/issues/projet-ccm2/twitch-event-listener) | ![PRs](https://img.shields.io/github/issues-pr/projet-ccm2/twitch-event-listener) | ![Status](https://img.shields.io/badge/status-active-green) |
| [twitch-requester](https://github.com/projet-ccm2/twitch-requester) | *Twitch API interface* to retrieve streamer and viewer data | ![Issues](https://img.shields.io/github/issues/projet-ccm2/twitch-requester) | ![PRs](https://img.shields.io/github/issues-pr/projet-ccm2/twitch-requester) | ![Status](https://img.shields.io/badge/status-active-green) |
| [API](https://github.com/projet-ccm2/API) | *Central API Gateway* exposing RESTful endpoints for all clients | ![Issues](https://img.shields.io/github/issues/projet-ccm2/API) | ![PRs](https://img.shields.io/github/issues-pr/projet-ccm2/API) | ![Status](https://img.shields.io/badge/status-active-green) |

#### 🎯 Business Services
| Service | Description | Issues | PRs | Status |
|---------|-------------|--------|-----|--------|
| [achievement-management](https://github.com/projet-ccm2/achievement-management) | *Achievement management*: creation, validation, attribution and progression | ![Issues](https://img.shields.io/github/issues/projet-ccm2/achievement-management) | ![PRs](https://img.shields.io/github/issues-pr/projet-ccm2/achievement-management) | ![Status](https://img.shields.io/badge/status-active-green) |
| [user-management](https://github.com/projet-ccm2/user-management) | *User management*: profiles, authentication, authorizations | ![Issues](https://img.shields.io/github/issues/projet-ccm2/user-management) | ![PRs](https://img.shields.io/github/issues-pr/projet-ccm2/user-management) | ![Status](https://img.shields.io/badge/status-active-green) |
| [notification-handler](https://github.com/projet-ccm2/notification-handler) | *Multi-channel notification system* (Twitch, Discord, mobile) | ![Issues](https://img.shields.io/github/issues/projet-ccm2/notification-handler) | ![PRs](https://img.shields.io/github/issues-pr/projet-ccm2/notification-handler) | ![Status](https://img.shields.io/badge/status-active-green) |

#### 🤖 Support Services
| Service | Description | Issues | PRs | Status |
|---------|-------------|--------|-----|--------|
| [IA-manager](https://github.com/projet-ccm2/IA-manager) | *Artificial Intelligence*: automatic achievement generation and behavioral analysis | ![Issues](https://img.shields.io/github/issues/projet-ccm2/IA-manager) | ![PRs](https://img.shields.io/github/issues-pr/projet-ccm2/IA-manager) | ![Status](https://img.shields.io/badge/status-active-green) |
| [DB-gateway](https://github.com/projet-ccm2/DB-gateway) | *Database gateway*: secure and consistent CRUD operations | ![Issues](https://img.shields.io/github/issues/projet-ccm2/DB-gateway) | ![PRs](https://img.shields.io/github/issues-pr/projet-ccm2/DB-gateway) | ![Status](https://img.shields.io/badge/status-active-green) |
| [bucket-manager](https://github.com/projet-ccm2/bucket-manager) | *File management*: image storage, configurations, static resources | ![Issues](https://img.shields.io/github/issues/projet-ccm2/bucket-manager) | ![PRs](https://img.shields.io/github/issues-pr/projet-ccm2/bucket-manager) | ![Status](https://img.shields.io/badge/status-active-green) |

#### 🛠️ Infrastructure & DevOps
| Service | Description | Issues | PRs | Status |
|---------|-------------|--------|-----|--------|
| [shared-workflows](https://github.com/projet-ccm2/shared-workflows) | *GitHub Actions workflows*: reusable CI/CD pipelines and automation scripts | ![Issues](https://img.shields.io/github/issues/projet-ccm2/shared-workflows) | ![PRs](https://img.shields.io/github/issues-pr/projet-ccm2/shared-workflows) | ![Status](https://img.shields.io/badge/status-completed-brightgreen) |
| [terraformInfra](https://github.com/projet-ccm2/terraformInfra) | *Infrastructure as Code*: Terraform configurations for GCP deployment and resource management | ![Issues](https://img.shields.io/github/issues/projet-ccm2/terraformInfra) | ![PRs](https://img.shields.io/github/issues-pr/projet-ccm2/terraformInfra) | ![Status](https://img.shields.io/badge/status-completed-brightgreen) |

#### 🎨 Frontend & Applications
| Service | Description | Issues | PRs | Status |
|---------|-------------|--------|-----|--------|
| [front](https://github.com/projet-ccm2/front) | *Frontend application*: React web interface for streamers and viewers to manage achievements, with Capacitor for mobile web app | ![Issues](https://img.shields.io/github/issues/projet-ccm2/front) | ![PRs](https://img.shields.io/github/issues-pr/projet-ccm2/front) | ![Status](https://img.shields.io/badge/status-active-green) |
| [bot-discord](https://github.com/projet-ccm2/bot-discord) | *Discord Bot*: automated notifications and community management integration | ![Issues](https://img.shields.io/github/issues/projet-ccm2/bot-discord) | ![PRs](https://img.shields.io/github/issues-pr/projet-ccm2/bot-discord) | ![Status](https://img.shields.io/badge/status-active-green) |

### Data Diagram

![Data Diagram](../docs/data.png)

### Quick Links
- 📋 [All Issues](https://github.com/orgs/projet-ccm2/issues)
- 🔄 [All Pull Requests](https://github.com/orgs/projet-ccm2/pulls)
- 📈 [Project Board](https://github.com/orgs/projet-ccm2/projects)

## 📋 Project Structure

This organization repository contains:
- Project documentation
- Presentation resources
- Links to different system components

---

*Project developed as part of a training integrating Cloud Computing, Mobility and AI*
