# Phong_Model-OpenGL
This repository contains a C++ implementation of the Phong Lighting Model using OpenGL and GLFW. It allows you to illuminate 3D objects using the Phong shading technique and includes a feature to import and load models for rendering with the lighting model.

## Prerequisites
Before using this repository, ensure that you have the following prerequisites installed:

- C++ compiler (GCC, Clang, or Visual Studio C++)
- OpenGL
- GLFW (Graphics Library Framework)

## Importing and Loading Models
This repository includes a simple model importer to load 3D models in Wavefront OBJ format. To import and load a model for rendering, follow these steps:

1) Prepare your 3D model in Wavefront OBJ format (.obj file).

2) Copy the OBJ file into the models directory in this repository.

3) Open the main.cpp file in your preferred text editor.

4) Locate the line with the following code:
```
const std::string modelPath = "models/your_model.obj";

```
5) Replace "models/your_model.obj" with the relative path to your OBJ file.
6) Save the changes and rebuild the application.
```
g++ main.cpp -lglfw -lGL -o phong_lighting_model
```
7) Run the application again:
```
./phong_lighting_model
```
The Phong Lighting Model will now load and render your specified 3D model.

## Controls
The application provides the following controls:

- W/A/S/D: Move the camera forward/left/backward/right.
- Mouse Movement: Rotate the camera to change the view.
- Scroll Wheel: Zoom in/out.
- Q/E: Increase/decrease the specular exponent of the Phong lighting model (adjusts shininess).
- R: Reset the camera position and view.
- Esc: Close the application.

## Contributing
Contributions to this repository are always welcome. If you encounter any issues or have ideas for improvements, please feel free to open an issue or submit a pull request.

## License
This repository is licensed under the MIT License. Feel free to use and modify the code for your own projects.
