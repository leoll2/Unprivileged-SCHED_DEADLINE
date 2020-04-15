# Unprivileged-SCHED_DEADLINE

Set of patches for [**Linux Kernel**](https://github.com/torvalds/linux) and [**Linux PAM**](https://github.com/linux-pam/linux-pam), implementing a mechanism to 
to allow unprivileged (non-root) processes to use the SCHED\_DEADLINE real-time scheduling features, according to a tunable access policy.

It is based on the introduction of new resource limits, whose configuration can be specified in `limits.conf`.

Further details can be found [**here**](report.pdf).

## Setup

### Linux kernel

Apply `linux-kernel_arom.patch` to the kernel source, then `linux-kernel_leo.patch`, and finally recompile.

### Linux PAM

Apply `linux-pam_arom.patch` to the kernel source, then `linux-pam_leo.patch`, and finally recompile.

## Issues

Feel free to report any bug or request a new feature by opening an issue in this repository.
