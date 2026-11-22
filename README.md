
# 🍂 Falling Leaves Animation

A lightweight, customizable falling leaves animation component for React applications, built with **React, TypeScript, and HTML Canvas API**.

No animation libraries. No additional dependencies. Just download one file, add it to your project, and you're ready to go!

## ✨ Preview

<!-- Add your animation GIF or screenshot here -->
<!-- ![Falling Leaves Preview](./preview.gif) -->

## 🚀 Installation

No npm package installation required!

### 1. Download the Component

Download the latest `FallingLeaves.tsx` file from the [Releases](../../releases/latest) page.

### 2. Add It to Your Project

Place the downloaded file inside your components directory:

```text
your-project/
├── src/
│   ├── components/
│   │   └── FallingLeaves.tsx
│   └── App.tsx
```

### 3. Use It

Import the component and add it to your application:

```tsx
import FallingLeaves from "./components/FallingLeaves";

function App() {
  return (
    <>
      <FallingLeaves />

      <main>
        <h1>Welcome to Autumn 🍂</h1>
      </main>
    </>
  );
}

export default App;
```

That's it! Your falling leaves animation is ready.

> **Note:** The component uses Tailwind CSS utility classes for positioning. Make sure Tailwind CSS is configured in your project.

## ⚙️ Configuration

You can customize the animation using the following props:

| Prop | Type | Default | Description |
|---|---|---|---|
| `leafCount` | `number` | `25` | Number of leaves displayed |
| `opacity` | `number` | `0.5` | Overall leaf transparency (0–1) |
| `minSize` | `number` | `18` | Minimum leaf size in pixels |
| `maxSize` | `number` | `42` | Maximum leaf size in pixels |
| `fullScreen` | `boolean` | `true` | Whether the animation covers the entire viewport |
| `zIndex` | `number` | `40` | CSS stacking order of the canvas |
| `shapes` | `LeafShape[]` | All shapes | Select which leaf shapes to display |

## 🍁 Available Leaf Shapes

You can choose from five different leaf shapes:

| Shape | Description |
|---|---|
| `maple` | Classic maple leaf |
| `oak` | Oak leaf |
| `birch` | Birch leaf |
| `ginkgo` | Fan-shaped ginkgo leaf |
| `elm` | Elm leaf |

## 🎨 Customization Examples

### Customize Animation Density

```tsx
<FallingLeaves leafCount={50} />
```

### Change Leaf Size

```tsx
<FallingLeaves minSize={25} maxSize={60} />
```

### Adjust Transparency

```tsx
<FallingLeaves opacity={0.3} />
```

### Use Specific Leaf Shapes

```tsx
<FallingLeaves
  shapes={["maple", "oak", "ginkgo"]}
/>
```

### Disable Fullscreen Mode

```tsx
<div className="relative h-[500px]">
  <FallingLeaves
    fullScreen={false}
    leafCount={15}
  />
</div>
```

### Combine Multiple Options

```tsx
<FallingLeaves
  leafCount={40}
  opacity={0.4}
  minSize={20}
  maxSize={55}
  fullScreen={true}
  zIndex={10}
  shapes={["maple", "oak", "birch"]}
/>
```

## ⚡ Features

- **Canvas Rendering:** Smooth animation using the native HTML Canvas API.
- **Natural Movement:** Randomized falling speeds, rotation, and horizontal movement.
- **Scroll Interaction:** Leaves respond naturally to scrolling direction and intensity.
- **Five Leaf Shapes:** Multiple handcrafted leaf designs.
- **Responsive:** Automatically adjusts to window resizing.
- **Performance:** Uses `requestAnimationFrame` and pauses when the document is hidden.
- **Reusable:** Easy to integrate into any React application.

## 🛠️ Built With

- React
- TypeScript
- HTML Canvas API

## 📄 License

This project is licensed under the MIT License.
