# 📱 Simple Kernel Builder

An automated GitHub Action for compiling Android kernels with integrated KernelSU support.

---

## 🚀 Getting Started

1. **Fork** this repository.
2. Open `.github/workflows/build.yml` and look at the `env:` section at the top.
3. Edit the **Links**, **Branches**, and **Flags** to match your device.
4. Go to **Actions** -> select **Build Kernel** -> click **Run workflow**.

---

## ⚙️ Configuration Flags (In `build.yml`)

| Variable | Description |
| :--- | :--- |
| `KERNEL_SOURCE` | Link to your kernel repository. |
| `KERNEL_BRANCH` | The branch you want to build. |
| `CLANG_URL` | Link to Clang toolchain (git or tar.gz). |
| `AK3_SOURCE` | AnyKernel3 repository link. |
| `KSU_SOURCE` | KernelSU setup script link. |
| `BUILD_HOST` | Name of your kernel (used for the zip name). |
| `FETCH_KSU_APK` | Set to `true` to bundle the KSU Manager APK in your release. |

---

**Made with ❤️ by [@dantepaulxd](https://github.com/dpxdoss)**
