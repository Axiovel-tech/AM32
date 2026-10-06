# Axiovel AM32 fork

ESC firmware for the AxioLight drone (AT32F421 ESC, target `AXIOLIGHT_F421`
in `Inc/targets.h`).

## Build

```bash
make arm_sdk_install
make AXIOLIGHT_F421
```

Output: `obj/AM32_AXIOLIGHT_F421_<version>.bin`.

## Branches

- `main` mirrors upstream `am32-firmware/AM32`. Never commit Axiovel work to it.
- `AV-x.yy` is upstream release tag `vx.yy` plus the Axiovel commits (the
  target and this file).

To take a new upstream release, branch `AV-x.yy` from the new tag and
cherry-pick the Axiovel commits from the previous `AV` branch. Do not merge
upstream into an existing `AV` branch.
