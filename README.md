# #️ Simple Kernel Builder

An GitHub Action for compiling Android kernels with integrated KernelSU support. 
Optimized for modern runners and multi-device compatibility.

---

🚀 Getting Started

### 1. Setup
* **Fork** this repository to your GitHub account.
* Then edit the build.yml of your forked repo OR
* Navigate to the **Actions** tab in your forked repo.
* Select **Build Kernel** from the workflow list on the left.

### 2. Launching a Build
Click **Run workflow** and provide your specific details:

* **Kernel Source / Branch:** Link of your kernel repository.
* **Clang Link:** tar.gz direct link or a Git repo.
* **AnyKernel Link / Branch:** Your AnyKernel3 repository.

* **KernelSU Link:** Setup script Link
* e.g., KSU Official, KSU Next, WildKSU.
* **Leave empty to skip KSU integration.**

**Click "Run workflow" to begin the process.**

---

## 📝 Key Features & Details

* **Smart Naming:**
* automatically generates a professional filename:
`{KernelName}_{KSU-Version}_{Device}_{Date-Time}.zip`.

* **Automatic KSU Detection:**
Automatically identifies KSU type form link and
fetches the matching Manager APK and upload with releases.

* **Universal Image Finding:**
Automatically detects the compiled kernel image
(Image.gz, Image.gz-dtb, etc.) regardless of device architecture.

* **Draft Releases:**
by Default builds are uploaded as **Draft Releases**.
You can review them before making them public.

* **Native Logging:**
Full compilation logs are available directly
in the GitHub Actions console for easy troubleshooting.

---

**Made with ❤️ by @dantepaulxd**
