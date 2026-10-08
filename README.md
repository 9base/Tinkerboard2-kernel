> [!NOTE]
> **9base status: Preserved** · **Lifecycle: archived reference copy.**
>
> This is a historical fork of [TinkerBoard2/kernel](https://github.com/TinkerBoard2/kernel).
> 9base retains it for provenance and reference and does not actively maintain it.
> Upstream source and inherited authorship remain attributed to their original contributors.

# Tinkerboard2-kernel — 9base preservation notes

## Role and historical evidence

This is the Tinker Board 2/RK3399 vendor Linux kernel component. The default
`linux4.4-rk3399-debian10` branch and the other 4.4 branch were identical to their
same-named upstream branches in the 8 October 2026 audit.

The non-default [linux4.19-rk3399-debian10 branch](https://github.com/9base/Tinkerboard2-kernel/tree/linux4.19-rk3399-debian10)
contains exactly one fork-only commit,
[8d7aced](https://github.com/9base/Tinkerboard2-kernel/commit/8d7aced868a7e6f4b06965211b91773ae341bd4a),
authored by Suleyman Poyraz (Zaryob) on 18 September 2022. It adds 35 README lines
about a vanilla-kernel build experiment; it changes no kernel source. The
historical snippet mixes `rk3288` and `rk3399` device-tree names and different
built/copied DTB filenames, and includes historical LTS commentary. It is
preserved on that branch as unverified historical documentation, not as a
validated current build recipe. The 4.19 branch compared 1 commit ahead and
3,471 behind upstream at the audit snapshot.

The full account-filtered inherited-history query for 4.19 failed at GitHub;
the successful exact comparison identifies the sole fork-only README commit,
but does not exhaustively resolve all inherited author identities.

The original upstream [README](README), [COPYING](COPYING), credits and source
history are retained unchanged. Consult the upstream documentation in its
historical version context; this curation has not validated a kernel build.

## Tinker Board 2 platform family

| Layer | Preserved 9base repository |
| --- | --- |
| Linux checkout manifests | [Tinkerboard2-manifest](https://github.com/9base/Tinkerboard2-manifest) |
| Linux kernel | [Tinkerboard2-kernel](https://github.com/9base/Tinkerboard2-kernel) |
| U-Boot bootloader | [Tinkerboard2-uboot](https://github.com/9base/Tinkerboard2-uboot) |
| Buildroot build system | [Tinkerboard2-buildroot](https://github.com/9base/Tinkerboard2-buildroot) |
| Debian/rootfs scripts | [Tinkerboard2-debian](https://github.com/9base/Tinkerboard2-debian) |
| Rockchip firmware and loaders | [Tinkerboard2-rkbin](https://github.com/9base/Tinkerboard2-rkbin) |
| Poky/OpenEmbedded/BitBake | [yocto-poky](https://github.com/9base/yocto-poky) |
| Android checkout manifests | [Tinkerboard2Android-manifest](https://github.com/9base/Tinkerboard2Android-manifest) |

The [Linux release manifest](https://github.com/9base/Tinkerboard2-manifest/blob/linux4.19-rk3399-debian10/default.xml) explicitly names the kernel, U-Boot,
Buildroot, Debian, rkbin and yocto-poky components. Its remote still points to
`TinkerBoard2`, not these 9base forks; it does not automatically select 9base's
historical Debian fix. This family is only a retained subset of the vendor's
larger source graph, not a self-contained complete BSP checkout.

The Android manifests concern the same board family but target a separate
`TinkerBoard2-Android` source graph; they do not establish use of these 9base
Linux components.

## Historical note

These preservation notes were reconstructed on **8 October 2026** from the
repository tree, exposed branches, commit history and upstream comparisons.
They are new archival documentation, not evidence that this explanation existed
at the historical fork date. The original reason for retention or any deployment
is not established by the inspected record. No contemporary build, support or
upstream synchronization commitment is implied.

The original upstream [README](README) is retained as a separate,
unchanged file. Its historical content and other README variants are preserved.
