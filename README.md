# 🌐 TerpWheel 3D

A web and mobile-compatible interactive 3D terpene wheel for mapping sensory profiles of cannabis and other aromatic products — with future support for **React Native** and direct integration with **[MyGrow.app](https://mygrow.app)**.

---

## 🎯 Purpose

This project aims to create a unique **3D sensory interface** where users can interact with an orb-shaped terpene wheel. By dragging intensity points around the sphere, users define the aromatic and flavor profile of a product in a dynamic and visual way.

The interface outputs a structured JSON object representing the intensity and presence of various sensory clusters — like citrus, floral, earthy, and sweet — useful for research, phenotyping, or consumer feedback.

---

## 📲 React Native Goal

The long-term objective is to enable **full integration into MyGrow.app**, which is built with **React Native + Expo**.

To support this, the 3D interface will be built using:
- [Three.js](https://threejs.org/) with [react-three-fiber](https://github.com/pmndrs/react-three-fiber)
- Future React Native support via [`expo-three`](https://github.com/expo/expo-three) or [`react-three-fiber/native`](https://github.com/pmndrs/react-three-fiber/blob/main/packages/fiber/README.md#react-native)

The 3D wheel will work both:
- 📱 as a module inside the mobile app
- 🌐 as a standalone web app for quick access and evaluation

---

## 🔄 Integration with MyGrow.app

Planned integration features include:
- Attach terpene profiles to specific plant harvests
- Allow growers to evaluate buds post-harvest using the 3D wheel
- Send profile data to the backend using MyGrow API
- Display terpene profile visually within the plant history timeline

---

## 🧱 Tech Stack

- [React](https://react.dev/)
- [Three.js](https://threejs.org/) via `@react-three/fiber`
- [Vite](https://vitejs.dev/)
- [Tailwind CSS](https://tailwindcss.com/) (for web styling)
- [Zustand](https://github.com/pmndrs/zustand) (state management)
- [Expo](https://expo.dev/) (for future React Native support)

---

## ✨ MVP Goals

- [x] Render a 3D orb with terpene anchor points (e.g. citrus, floral, herbal)
- [x] Allow dragging from center to activate intensity vectors
- [x] Generate a triangulated "web" from selected points
- [x] Export sensory profile as JSON
- [ ] Add mock API integration with MyGrow
- [ ] Build proof of concept for React Native using `expo-three`

---

## 📦 Getting Started (Web)

```bash
npm create vite@latest terpwheel-3d -- --template react
cd terpwheel-3d
npm install
npm install three @react-three/fiber @react-three/drei
