# 📱 Simple Kernel Builder

An automated GitHub Action for compiling Android kernels. Developed by **@dantepaulxd**

-----

# 🚀 Guide

### 1\. Setup

  * **Fork** this repository to your own account.
  * Navigate to the **Actions** tab in your forked repo.
  * On the left sidebar, click on **Build Kernel**.
  * Click **Enable Actions** if it is your first time.

### 2\. Build

Click **Run workflow** and fill in the following fields:

  * **Kernel Source:** The link to your kernel repository.
  * **Kernel Branch:** The branch name you want to build (e.g., `sixteen-qpr2`).
  * **Clang Source:** The toolchain link (AOSP tar.gz or Git link).
  * **KSU Source:** The KernelSU setup script link (**Leave empty to skip KSU**).
  * **AnyKernel3 Source:** Your preferred AnyKernel3 repository for zipping.
  * **Output Type:** Select between **Zip**, **boot.img**, or **Both**.

**Click "Run workflow" to start building.**

-----

# 📝 Details

  * **Draft Release:** Once the build is finished, a **Draft** will be created in your [Releases](https://www.google.com/search?q=https://github.com/settings/replaceme) page. You must manually publish it to make it public.
  * **Logs:** If the build fails, a `Failure-Log` will be available in the **Artifacts** section of the Action run for troubleshooting.
  * **Cleanup:** The workspace is automatically cleaned after every run to keep the environment fast and safe.

-----

**Made with ❤️ by @dantepaulxd**
