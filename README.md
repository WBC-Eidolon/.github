# 🌀 Eidolon

Welcome to **Eidolon**, the next-generation modular platform for building scalable, multi-platform applications.  

Eidolon unifies **frontend, backend, plugins, and shared tools** into a single ecosystem — giving you **flexibility, speed, and power** to build modern software without compromises.

---

## ✨ Why Eidolon?

- **Modular & Scalable** – Add or remove features with plug-and-play frontend and backend plugins.  
- **Multi-Platform Ready** – Web, desktop (Tauri/Electron), local or cloud backend deployment.  
- **Shared Intelligence** – Centralized BFF layer (`codex`) ensures type-safe API communication across all layers.  
- **Future-Proof Architecture** – Easily migrate backend plugins to high-performance languages like Go or Rust without breaking the system.  
- **Developer Friendly** – CLI tools (`touchstone`) and UI components (`lumina`) make development fast, consistent, and maintainable.

---

## 🚀 Layers of Eidolon

### Frontend
- **Phantasm** – The main React shell powering the user experience.  
- **Lumina** – A polished, prebuilt UI component library.  
- **Frontend Plugins** – Extend functionality on-demand:  
  - **Spectroscope** – PDF templating engine  
  - **Conflux** – CRM & workspace manager  
  - **Gold** – Payment & cloud storage management  
  - **Ritual** – Automated workflows & macros  

### Backend
- **Liminal** – Core NestJS logic powering your apps  
- **Shade & Revenant** – Local & cloud backend deployment blueprints  
- **Backend Plugins** – High-performance microservices:  
  - **Tether** – File abstraction layer  
  - **Harbinger** – Synchronization engine  
  - **Locksmith** – Encryption and certificate management  

### Shared Packages
- **Codex** – The brain: shared types, callbacks, and API transformations  
- **Lumina** – UI components for consistent design across apps  

### Developer Tools
- **Touchstone** – CLI for scaffolding, building, and managing your projects  

---

## 🌐 Architecture at a Glance

```mermaid
graph TD
subgraph Frontend
phantasm --> lumina
phantasm --> frontend-plugin-spectroscope
phantasm --> frontend-plugin-conflux
phantasm --> frontend-plugin-gold
phantasm --> frontend-plugin-ritual
end

subgraph Backend
liminal --> shade-revenant
liminal --> backend-plugin-tether
liminal --> backend-plugin-harbinger
liminal --> backend-plugin-locksmith
end

Frontend --> codex
Backend --> codex
