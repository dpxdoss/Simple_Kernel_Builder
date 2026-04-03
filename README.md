**📱 Simple Kernel Builder**

An automated GitHub Action for compiling Android kernels with integrated KernelSU support.

**🚀 Getting Started**
1. **Fork** this repository.
2. Open `.github/workflows/Build Kernel.yml` in your fork repo.
3. Edit the **Links**, **Branches**, and **Configuration Flags** to match your device.
4. Go to **Actions** -> select **Build Kernel** -> click **Run workflow**.

**⚙️ Configuration Flags**

| Flag Name | Default | Description |
| :--- | :--- | :--- |
| `BUILD_HOST` | `ReviveMeJett` | Prefix for the ZIP and Release name. |
| `BUILD_USER` | `dantepaulxd` | Prefix for the kernel version info. |
| `USE_LLVM` | `1` | `1` to build with Clang/LLVM, `0` for GCC. |
| `USE_KSU` | `true` | Set to `false` to skip KernelSU patching. |
| `FETCH_KSU_APK` | `true` | Add latest matching KSU manager apk in release page. |
| `INCLUDE_KSU_VERSION`| `true` | Set to `false` to skip KSU version tag in file name. |
| `NO_ERROR_ON_MISMATCH` | `y` | Ignores non-critical warnings to prevent build failure. |
| `POST_AS_DRAFT` | `true` | Uploads Releases as Draft (private). Set to `false` for Public. |
| `INCLUDE_DATE` | `true` | Adds `DDMMYY-HHMM` stamp to the filename. |
| `EXTRA_MAKE_FLAGS` | `""` | Add extra arguments here (e.g., `"LLVM_IAS=1"`). |

**Made with ❤️ by [Dante](https://github.com/dpxdoss)**
