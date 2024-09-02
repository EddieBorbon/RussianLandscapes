# 🎨 Russian Memories: An Artistic Web Experience

This web project showcases a collection of photos I took during my stay in Russia. Each time you load the page, a photo is randomly selected and displayed using a custom particle system, creating a unique visual experience for every visitor.

Developed with **Three.js**, this interactive project turns each photograph into a stunning particle-based artwork.

## 🌟 Features
- Display of **random photos** from my collection taken in Russia.
- Custom **particle system** that dynamically represents each image.
- Interactive 3D environment with **camera controls**.

## 🛠️ Project Setup

1. Clone the repository.
2. Ensure you have a local server to view the project (you can use **Live Server** in Visual Studio Code or any preferred server setup).
3. Open `index.html` in a browser to experience the project.

## ⚙️ Code Overview

### Key Components

- **Three.js**: This library is used to create and display the 3D graphics. It allows for rendering the particle system and handling camera controls.

- **Shaders**: Custom vertex and fragment shaders are used to process the particles. The shaders define how each particle is displayed based on its color and position.

- **Particle System**: Each photograph is broken into pixels, and each pixel is represented as a particle in a 3D space. The particle's position and color are determined by the pixel's data.

### How It Works

- **Initialization**:
  The `init()` function sets up the scene, camera, and controls, and loads an image to process.

- **Scene Creation**:
  `createScene()` initializes the Three.js scene, camera, and renderer. The renderer is used to display the particles on the webpage.

- **Controls Setup**:
  `createControls()` configures the camera controls, allowing users to interact with the scene using rotation, zoom, and pan.

- **Image Processing**:
  `createPixelData(imgsrc)` loads an image and processes its pixels. The pixel data is used to create the particle system where each particle's position and color are derived from the image.

- **Particle Creation**:
  `createParticles()` generates the particles based on the processed image data. The particles are added to the scene to create the visual effect.

- **Animation Loop**:
  `tick()` is the animation loop that continuously updates and renders the scene. It also updates the shader's amplitude to create dynamic visual effects.

- **Responsive Design**:
  `onWindowResize()` adjusts the camera and renderer settings when the window is resized, ensuring the display remains consistent.

## 🎨 Artistic Concept

This project transforms simple photographs into dynamic, particle-based compositions. Each photo is divided into pixels, and each pixel is transformed into a 3D particle based on its color intensity. The images represent not just moments in time but evoke a sense of randomness and fragmentation, reflecting how memories change over time.

## 🌐 Live Demo

Check out the project live: [Russian Memories Demo](https://eddieborbon.com/russian_landscapes/index.html)

## 📧 Contact

Feel free to reach out with any questions or suggestions:

- **Developer**: Eddie Jonathan Garcia Borbon
- 📧 **Email**: [your-email@example.com](mailto:your-email@example.com)

Enjoy exploring Russia through art! 🌍✨
