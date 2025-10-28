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

### Mobile Development
- **Flutter** or **React Native** for mobile application
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

![Architecture Diagram](./docs/architecture.png)

*Add your architecture diagram in the `docs/` folder with the name `architecture.png`*

### Microservices

The **StreamQuest** project is structured in microservices deployed on **Google Cloud Platform** with **Cloud Run**:

#### 🔗 Core Services
- **[twitch-event-listener](https://github.com/projet-ccm2/twitch-event-listener)**  
  *Listens to real-time Twitch events* (chat messages, subscriptions, donations)

- **[twitch-requester](https://github.com/projet-ccm2/twitch-requester)**  
  *Twitch API interface* to retrieve streamer and viewer data

- **[API](https://github.com/projet-ccm2/API)**  
  *Central API Gateway* exposing RESTful endpoints for all clients

#### 🎯 Business Services
- **[achievement-management](https://github.com/projet-ccm2/achievement-management)**  
  *Achievement management*: creation, validation, attribution and progression

- **[user-management](https://github.com/projet-ccm2/user-management)**  
  *User management*: profiles, authentication, authorizations

- **[notification-handler](https://github.com/projet-ccm2/notification-handler)**  
  *Multi-channel notification system* (Twitch, Discord, mobile)

#### 🤖 Support Services
- **[IA-manager](https://github.com/projet-ccm2/IA-manager)**  
  *Artificial Intelligence*: automatic achievement generation and behavioral analysis

- **[DB-gateway](https://github.com/projet-ccm2/DB-gateway)**  
  *Database gateway*: secure and consistent CRUD operations

- **[bucket-manager](https://github.com/projet-ccm2/bucket-manager)**  
  *File management*: image storage, configurations, static resources

### Data Diagram

```markdown
# TODO: Data Diagram
```

## 📋 Project Structure

This organization repository contains:
- Project documentation
- Presentation resources
- Links to different system components

---

*Project developed as part of a training integrating Cloud Computing, Mobility and AI*
