# 🎩 Houdini ARM Translation Master Bundle

This package contains the **Houdini** translation layer components extracted from the **FydeOS (Android 11/13)** vendor image. It enables running ARM/ARM64 applications on x86_64 systems.

## 📂 Package Structure

- **/bin**: `houdini` and `houdini64` binary interpreters.
- **/lib**: 32-bit `libhoudini.so` and native ARM runtime libraries.
- **/lib64**: 64-bit `libhoudini.so` and native ARM64 runtime libraries.
- **/etc/binfmt_misc**: Kernel registration rules for transparent execution.

## ⚙️ Deployment Guide

### 1. Permissions
Ensure all binaries and shared libraries have execution permissions:
```bash
chmod +x ./bin/houdini*
chmod +x ./lib/libhoudini.so
chmod +x ./lib64/libhoudini.so
