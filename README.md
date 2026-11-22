
# 🍂 Falling Leaves Animation

A lightweight, reusable falling leaves animation built with **React, TypeScript, and the HTML Canvas API**.

This project creates a natural falling leaves effect with smooth animations, randomized movement, and optimized canvas rendering — without relying on third-party animation libraries.

## ✨ Features

- 🍂 Smooth and natural falling leaves animation
- ⚡ Lightweight rendering using HTML Canvas API
- 🎲 Randomized leaf positions, rotations, and movement
- ♻️ Reusable React component
- 📱 Responsive canvas that adapts to different screen sizes
- 🚀 No external animation dependencies
- 🎨 Customizable animation behavior

## 🛠️ Tech Stack

- React
- TypeScript
- HTML Canvas API

## 📦 Installation

Clone the repository:

```bash
git clone YOUR_REPOSITORY_URL
```

Navigate to the project directory:

```bash
cd falling-leaves-animation
```

Install dependencies:

```bash
npm install
```

## 🚀 Usage

Import the `FallingLeaves` component into your React application:

```tsx
import FallingLeaves from "./components/FallingLeaves";

export default function App() {
  return (
    <main>
      <FallingLeaves />
    </main>
  );
}
```

## ⚙️ How It Works

The animation uses the HTML Canvas API to draw and animate falling leaves.

Each leaf has randomized properties such as:

- Position
- Size
- Rotation
- Falling speed
- Horizontal movement

The animation loop continuously updates leaf positions and redraws the canvas to create a smooth and natural effect.

## 🎯 Motivation

I wanted to create a seasonal falling leaves effect without depending on third-party animation packages.

Instead of installing an existing library, I decided to build a custom, reusable React component using the Canvas API.

This gave me more control over the animation behavior, performance, and implementation.

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
