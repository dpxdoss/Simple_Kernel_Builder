# 📱 Simple Kernel Builder

An automated GitHub Action for compiling Android kernels with integrated KernelSU support.

---

## 🚀 Getting Started

1. **Fork** this repository.
2. (Optional) Edit the `env:` section in `.github/workflows/build.yml` to change your builder name or toggle features.
3. Go to **Actions** -> **Build Kernel** -> **Run workflow**.

---

## ⚙️ Configuration Guide

Users who fork this repo can customize these flags in the `env:` block:

| Flag Name | Default | Description |
| :--- | :--- | :--- |
| `BUILD_HOST` | `ReviveMeJett` | Prefix for the ZIP and Release name. |
| `BUILD_USER` | `dantepaulxd` | Name appearing in the kernel version info. |
| `USE_LLVM` | `1` | `1` to build with Clang, `0` for GCC. |
| `USE_KSU` | `true` | Set to `false` to skip KernelSU integration. |
| `NO_ERROR_ON_MISMATCH` | `y` | Skips minor compiler errors (useful for modern toolchains). |
| `POST_AS_DRAFT` | `true` | Creates a Draft Release by default. |
| `INCLUDE_DATE` | `true` | Adds timestamp to filename. |
| `INCLUDE_VERSION` | `true` | Adds auto-fetched kernel version (e.g. `v4.14.212`) to filename. |
| `EXTRA_MAKE_FLAGS` | `""` | Add extra flags here (Example: `"LLVM_IAS=1"`). |

---

## 📝 Features

* **Auto-Version Fetch:** Automatically reads the kernel version from your `Makefile`.
* **Smart Naming:** Filenames follow: `{Host}{Version}_{KSU}_{Device}_{Date}.zip`.
* **KSU Manager Bundling:** Identifies KSU type from link and bundles the correct Manager APK automatically.
* **Universal Build:** Supports Clang/LLVM by default and identifies boot images automatically.

---

**Made with ❤️ by [@dantepaulxd](https://github.com/dpxdoss)**
