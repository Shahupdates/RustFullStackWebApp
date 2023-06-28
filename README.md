# RustFullStackWebApp

RustFullStackWebApp is a web application built using Rust and the Seed framework. It provides a browser-based frontend UI that interacts with a backend REST API. The application allows users to manage tasks and displays them in a user-friendly interface.

## Project Structure

The project follows a Cargo workspace structure with two crates: `backend` and `frontend`. The `backend` crate contains the code for the backend server, which includes a database layer and REST API implementation. The `frontend` crate contains the code for the browser-based frontend UI, implemented using the Seed framework.

The project is organized as follows:

- `backend/`: Contains the backend server code, including the database layer and REST API implementation.
- `frontend/`: Contains the frontend UI code implemented using the Seed framework.
- `src/`: Contains shared structs and models used by both the backend and frontend.

## Getting Started

To run the MyProject application locally, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/shahupdates/rustfullstackwebapp
   cd MyProject
   ```

2. Build the backend and frontend:
   ```
   cargo build -all
   ```
3. Build the wasm package for the frontend:
   ```
   rustup target add wasm32-unknown-unknown
   ```
4. Install the required wasm toolchain:
   ```
   rustup target add wasm32-unknown-unknown
   ```
5. Build the wasm package for the frontend:
   ```
   cd frontend
   wasm-pack build --target web --out-name package --dev
   ```
6. Start the backend server:
   ```
   cargo run -p backend --bin backend
   ```
7. Serve the frontend using a web server:
   ```
   cd frontend
   microserver
   ```
8. Open your browser and navigate to ```http://localhost:9090``` to access the MyProject application.

## Project Dependencies
The project relies on the following dependencies:

Backend:
* Diesel: Provides ORM functionality and database connectivity.
* Rocket: A web framework for building the backend REST API.
* serde: A serialization and deserialization library for working with JSON data.
Frontend:
* Seed: A web framework for building browser-based frontend UIs in Rust.
* wasm-bindgen: Enables interoperability between Rust and JavaScript in the browser.
* web-sys: Provides Rust bindings to Web APIs for browser interaction.
For a complete list of dependencies, refer to the Cargo.toml files in the respective crates (backend/Cargo.toml and frontend/Cargo.toml).


Acknowledgements
The MyProject application was built with the help of the following libraries and frameworks:

* Seed: The web framework used for building the frontend UI.
* Rocket: The web framework used for building the backend REST API.
* Diesel: The ORM used for database connectivity.
* serde: The serialization and deserialization library for working with JSON data.
* wasm-pack: The tool used for building the frontend Rust code into WebAssembly.
