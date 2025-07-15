# 🚘 DriverCoreOS

**DriverCoreOS** is a modular, open-source in-car system designed to enhance vehicle telemetry, navigation, driving modes, media control, and more—targeted at motorsport, enthusiast driving, and custom automotive setups.

> 🧩 Designed for **flexibility**, **extensibility**, and **hardware abstraction**, DriverCoreOS is composed of multiple components across ESP32 microcontrollers, Raspberry Pi interfaces, and a custom NixOS image for optimal boot-time and reproducibility.

---

## 🧱 Project Architecture

This repository serves as the **main entry point** for the entire project. It contains links to the submodules that make up the different parts of the ecosystem:

```
.
├── repos/
│   ├── esp32/		# ESP32 firmware for telemetry, LEDs, GPS, etc.
│   ├── rpi/		# Raspberry Pi UI, plugins, and driving logic
│   ├── nixos/		# Custom OS image built with Nix
│   └── installer/	# Setup & flashing tool for onboard installation
├── tools/		# Flake-based dev environment + utility scripts
└── docs/		# Documentation hub (architecture, dev guide, etc.)
```

---

## 📚 Documentation

For complete technical documentation, architecture diagrams, installation instructions, and development guides, visit the [`📖 docs/`](./docs/README.md)

---

## 🧠 About the Project

DriverCoreOS is developed by the **[DriverCoreOS-Team](https://github.com/DriverCoreOS-Team)** and welcomes contributors who want to extend in-car systems through open hardware and software development.

---

## 📦 Submodules & Repositories

| Repository | Description |
|------------|-------------|
| [`repos/esp32`](./repos/esp32)        | ESP32 firmware: OBD-II, GPS zones, LED feedback, plugins |
| [`repos/rpi`](./repos/rpi)            | Raspberry Pi app: media UI, telemetry, maps, plugins     |
| [`repos/nixos`](./repos/nixos)        | Custom NixOS image for Raspberry Pi                      |
| [`repos/installer`](./repos/installer)| Installation scripts and flashing tools                  |
| [`tools`](./tools)                    | Flake devshell and helper scripts                        |
| [`docs`](./docs)                      | Documentation, setup, and architecture guides            |

---

## 🛠️ Getting Started

Clone the project and all submodules:

```bash
git clone --recursive https://github.com/DriverCoreOS-Team/DriverCoreOS.git
cd DriverCoreOS
nix develop ./repos/tools
```

> For setup help, see [`docs/INSTALL.md`](./docs/INSTALL.md) or the [`installer`](./repos/installer) repo.

---

## 📜 License

This project is licensed under the **MIT License**.  
Feel free to fork, use, and contribute to the project.

---

## 🤝 Contributions

All contributions are welcome! Check out the [`docs/CONTRIBUTING.md`](./docs/CONTRIBUTING.md) (coming soon) for guidelines.
