# 📱 Universal Kernel Builder

An GitHub Action for compiling Android kernels with integrated KernelSU support. 
Optimized for modern runners and multi-device compatibility.

---

## 🚀 Getting Started

### 1. Setup
* **Fork** this repository to your GitHub account.
* Navigate to the **Actions** tab in your forked repo.
* Select **Build Kernel** from the workflow list on the left.
* Click **Enable Actions** if prompted.

### 2. Launching a Build
Click the **Run workflow** dropdown and provide your specific details:

* **Kernel Source / Branch:** Link of your kernel repository.
* **Clang Link:** tar.gz direct link or a Git repo.
* **AnyKernel Link/Branch:** Your AnyKernel3 repository.

* **KernelSU Link:** Setup script Link
* e.g., KSU Official, Next, or WildKSU. **Leave empty to skip KSU integration.**

**Click "Run workflow" to begin the process.**

---

## 📝 Key Features & Details

* **Smart Naming:**
* The workflow automatically generates a professional filename: `{KernelName}_{KSU-Version}_{Device}_{Date-Time}.zip`.
* **Automatic KSU Detection:**
* Automatically identifies if you are using Official KernelSU or KernelSU-Next and fetches the matching Manager APK.
* **Universal Image Finding:**
* Automatically detects the compiled boot image (Image.gz, Image.gz-dtb, etc.) regardless of device architecture.
* **Draft Releases:**
* Finished builds are uploaded as **Draft Releases**. You can review them before making them public.
* **Native Logging:**
* Full compilation logs are available directly in the GitHub Actions console for easy troubleshooting.
* **Node.js 24 Ready:**
* Uses the latest `actions/checkout@v5` to ensure compatibility with modern GitHub runners.

---

**Made with ❤️ by @dantepaulxd**
