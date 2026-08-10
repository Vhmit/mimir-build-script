## Mimir kernel script

- Checks dependencies before starting the build.
- Uses the `-z` option if you prefer it to be packed with AnyKernel.
- Uses the `-z` + `-ksu` option in case you want to distinguish the file using KernelSU.
- Uploads error logs to rustbin.
- Uploads the packed kernel to gofile if you prefer.
- Sends you the sha256sum for verification.
- Even if the upload link fails, it indicates the directory where the compiled kernel is located.

## How to use

```
wget https://raw.githubusercontent.com/Vhmit/mimir-build-script/v4.x-clang/build.sh
```

```
chmod +x build.sh && ./build.sh $DEVICE
```

## Notes

- The branch corresponds to the kernel version for which it is adapted.
- Change the kernel image to look for in the script if you do not use Image.gz-dtb.
- Before adapting it for your use, make sure to change the AnyKernel variables, as well as the locations of your defconfig and compiler, if necessary.
