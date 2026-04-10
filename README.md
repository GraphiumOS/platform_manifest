# GraphiumOS Platform Manifest

This repository contains the **platform manifest** for GraphiumOS.

It defines all core source repositories, remotes, and project structure required to initialize, sync, and build the GraphiumOS operating system.

---

## 🧬 About GraphiumOS

GraphiumOS is a **minimal, performance-focused, and customizable graphene-based operating system** designed for clean system behavior and developer control with aim to provide customised features.
---

## ⚙️ Usage

### 🔹 Initialize repo

```bash
repo init -u https://github.com/GraphiumOS/platform_manifest.git
```

### 🔹 Sync source

```bash
repo sync -c -j$(nproc --all)
```

---

## 🧱 Structure

The manifest includes:

* AOSP base repositories
* GraphiumOS custom forks
* Device-specific configurations
* Kernel and vendor sources

---

## 🔧 Customization

GraphiumOS overrides selected upstream projects with custom implementations such as:

* frameworks/base
* packages/apps/Settings
* SystemUI and core services

---

## 📦 Build

After syncing sources:
Example: building for emulator "sdk_phone64_x86_64"

```bash
source build/envsetup.sh
lunch sdk_phone64_x86_64
m -j$(nproc --all)
```

---

## 🛠 Requirements

* Linux (Ubuntu/Debian recommended)
* Minimum 16GB RAM (32GB recommended)
* At least 200GB free storage


---

## 🚧 Status

* GraphiumOS is currently under active development.
* GraphiumOS is ready to use.

---

## 🤝 Contributing

Contributions, suggestions, and improvements are welcome.

---

## 📜 License

This project follows the licensing terms of the respective upstream sources (AOSP and other components).

---

## 🔗 Related

* GraphiumOS organization: https://github.com/GraphiumOS

---
