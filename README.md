# 📱 Simple Kernel Builder

An automated GitHub Action for compiling Android kernels with integrated KernelSU support.

**Developed by [@dantepaulxd](https://github.com/dpxdoss)**

---

## 🚀 Getting Started

1. **Fork** this repository.
2. (Optional) Edit the `env:` section in `build.yml` to change your builder name or toggle features.
3. Go to **Actions** -> **Build Kernel** -> **Run workflow**.

---

## ⚙️ Configuration Flags

| Flag Name | Default | Description |
| :--- | :--- | :--- |
| `BUILD_HOST` | `ReviveMeJett` | Prefix for the ZIP and Release name. |
| `BUILD_USER` | `dantepaulxd` | Name appearing in the kernel version info. |
| `USE_LLVM` | `1` | `1` for Clang, `0` for GCC. |
| `USE_KSU` | `true` | Toggle KernelSU integration. |
| `FETCH_KSU_APK` | `true` | Download & include KSU Manager APK in release. |
| `NO_ERROR_ON_MISMATCH` | `y` | Skips minor compiler errors. |
| `POST_AS_DRAFT` | `true` | Creates a Draft Release. |
| `INCLUDE_DATE` | `true` | Adds a timestamp to the filename. |
| `EXTRA_MAKE_FLAGS` | `""` | Add extra flags here. |

---

## 📝 Features

* **Auto-KSU Versioning:** Fetches the latest KernelSU/Next version from GitHub API for professional naming.
* **Smart APK Fetching:** Option to automatically include the matching KSU Manager APK in your release.
* **Professional Naming:** `{Host}_{KSU-Version}_{Device}_{Date}.zip`.
* **Universal Build:** Automatically identifies kernel images and supports modern toolchains.

---

**Made with ❤️ by @dantepaulxd**
