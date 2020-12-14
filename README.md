# cjktty-patches

Patches from [Gentoo-zh/linux-cjktty](https://github.com/Gentoo-zh/linux-cjktty) with minor changes.

**NOTE**: Starting from 5.10, the kernel config `CONFIG_FONT_16x16_CJK` has been renamed to `CONFIG_FONT_CJK_16x16`.

## CHANGES

### 20201214 / 5.10

- Resync for linux-5.10.y
- Update glyphs for some Chinese punctuation marks
- Support display rotation
- Support `setfont` (NOTE: different font size can cause issues with this patch which expect to work with `8x16 / 16x32` font)
- Fix display for some single width characters
- Fix line wrap for double width characters (<https://github.com/zhmars/cjktty-patches/issues/1>)
- Workaround from <https://github.com/Gentoo-zh/linux-cjktty/commit/6caf83a638886220d1e1880c92e8b18243c3965a>
- Support `32x32` font for high resolution screens (experimental, make sure the font data patch is applied)

### 20200918 / 5.8.10

- Resync for linux-5.8.10
- Remove soft scrollback code support (upstream)
