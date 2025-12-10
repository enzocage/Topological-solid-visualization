# **🪐 Topological Shapes Visualization** 

View: https://topologic.netlify.app

10.12.2025 by [felixschmidt.org](http://felixschmidt.org)


A comprehensive, interactive 3D explorer for mathematical surfaces and topological shapes. This application visualizes over 50 complex parametric geometries using **Three.js**, allowing users to manipulate mathematical variables in real-time.

## **✨ Features**

* **Extensive Library:** Visualization of 50+ unique topological bodies, ranging from standard shapes (Möbius Strip, Torus) to complex surfaces (Boy's Surface, Kuen's Surface, Dini's Surface).  
* **Real-time Parametric Control:** Each shape has specific mathematical variables (radius, width, frequency, etc.) that can be adjusted via sliders to instantly reshape the geometry.  
* **Auto-Animation Mode:** An "Auto-Mode" toggle that modulates shape parameters using sine waves for hypnotic visual effects.  
* **Interactive 3D View:** Full OrbitControls allowing users to rotate, zoom, and pan around the object.  
* **Visual Customization:**  
  * Toggle between Solid and Wireframe modes.  
  * Adjustable lighting intensity.  
  * Adjustable rotation speed.  
* **Modern UI:** A responsive, glassmorphism-style interface overlay built with Tailwind CSS.

## **🚀 Technologies Used**

* **HTML5 / JavaScript (ES6+)**  
* [**Three.js**](https://threejs.org/) **(r128):** For WebGL 3D rendering.  
* [**Tailwind CSS**](https://tailwindcss.com/)**:** For styling the user interface.  
* **OrbitControls:** For camera interaction.

## **🛠️ Installation & Usage**

This project is a self-contained Single Page Application (SPA).

### **Prerequisites**

An active internet connection is required to load the libraries (Three.js and Tailwind) via CDN.

### **Running the App**

1. Save the code as `index.html`.  
2. Open the file in any modern web browser (Chrome, Firefox, Safari, Edge).  
3. **No local server required** (unless extending textures/assets).

## **🎛️ Controls**

The interface is divided into the 3D Canvas and the "Topology Explorer" UI panel.

| Control | Description |
| ----- | ----- |
| **Shape Select** | Choose one of the 50 predefined mathematical shapes from the dropdown. |
| **Prev/Next** | Use the arrows in the panel or the floating buttons at the bottom right to cycle shapes. |
| **Parameter Sliders** | Specific to each shape (e.g., `Radius`, `Twists`). Adjusts the math formula in real-time. |
| **Auto-Mode** | Checkbox. Automatically animates the parameters. |
| **Wireframe** | Checkbox. Switches the render material to a wireframe mesh. |
| **Light/Rotation** | Global sliders to control scene brightness and object auto-rotation speed. |
| **Mouse/Touch** | Click and drag to rotate the camera. Scroll to zoom. |

## **📐 Included Shapes (Excerpt)**

The application includes formulas for a wide variety of geometry, including:

* **Non-Orientable Surfaces:** Möbius Strip, Klein Bottle, Boy's Surface, Roman Surface.  
* **Minimal Surfaces:** Enneper Surface, Catalan Surface, Helikoid, Catenoid.  
* **Complex Manifolds:** Monkey Saddle, Whitney Umbrella, Cross-Cap.  
* **Nature-inspired:** Seashell (Schneckenhaus), Kidney Surface, Apple Surface.  
* **Mathematical Curiosities:** Gabriel's Horn, Lemniscate, Super-shapes.

## **📝 Code Structure**

The logic is contained within a single `<script>` block:

* `shapes`: An array of objects defining the `name`, mathematical `func` (parametric equation), and adjustable `params` for every object.  
* `createParametricGeometry`: A custom function that generates the 3D mesh based on the mathematical function selected.  
* `init()` / `animate()`: Standard Three.js boilerplate for scene setup and the render loop.

## **📄 License**

This project is open source and available for educational and personal use.
