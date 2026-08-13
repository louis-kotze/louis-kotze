### Hi, I'm Louis 👋

Senior full stack engineer based in South Africa. I build enterprise web applications by day and occasionally dig into the Linux kernel when my own hardware misbehaves.

**Personal site + writing:** [louiskotze.dev](https://louiskotze.dev)

#### Recent open source work

17 commits merged across five upstream projects, plus a `Reviewed-by` credit on another contributor's regulatory analysis.

- **[wpa_supplicant / hostap — 7 commits](https://git.w1.fi/cgit/hostap/log/?qt=author&q=Kotze)** — WiFi 7 multi-link (MLO) association fixes merged July–August 2026: stale per-link BSS entries, ML-probe channel scanning, per-link key clearing, duplicated association-request IEs, and a PMKSA-caching deauthentication fallback, with two hwsim regression tests. Found and reproduced against real AP hardware; ships in the 2.13 release.
- **[NetworkManager MR !2405](https://gitlab.freedesktop.org/NetworkManager/NetworkManager/-/merge_requests/2405)** — WiFi 7 MLO awareness for NetworkManager's background-scan logic: parses the AP-MLD address from the Multi-Link element so a single-AP MLO association keeps the relaxed scan cadence, eliminating scan-induced traffic stalls. Merged July 2026.
- **[wireless-regdb patches](https://lore.kernel.org/wireless-regdb/?q=f:loukot@gmail.com)** — Audit and patches for WiFi 6E/7 regulatory data: **7 commits merged** into `wens/wireless-regdb` across six jurisdictions (ZA ×2 / UA / HK / RU / KR / TG), each verified against the primary regulatory instrument. Plus a Reviewed-by on a peer patch widening RU 6 GHz channel width. Where a published instrument left a limit blank, I wrote to the national regulator (ARCEP Burkina Faso) and got a written ruling on the applicable 6 GHz limits before drafting the patch.
- **[rtw89 RF-calibration fix](https://lore.kernel.org/linux-wireless/20260416045536.817930-1-loukot@gmail.com/)** — RTL8922AU USB WiFi 7 timeout fix; in mainline, with 5 independent `Tested-by` tags across USB chipsets.
- **[cfg80211 MLO grammar fix](https://lore.kernel.org/linux-wireless/20260414122728.92234-1-loukot@gmail.com/)** — Error-message correction in `nl80211_validate_key_link_id`; in mainline.
- **[morrownr/rtw89 PR #76](https://github.com/morrownr/rtw89/pull/76)** — Same RF-calibration fix backported to the out-of-tree DKMS driver (merged 2026-04-24).
- **[Fedora bug 2458629](https://bugzilla.redhat.com/show_bug.cgi?id=2458629)** — Reproducer + root-cause analysis for a wpa_supplicant MLO reassociation race.
- **In review:** [a cfg80211 patch](https://lore.kernel.org/all/?q=f:loukot@gmail.com) improving the diagnostics when an association BSS lookup fails.

#### Elsewhere

- [louiskotze.dev](https://louiskotze.dev) — personal site, blog, and CV downloads
- [Prolific Studio](https://prolificstudio.co.za) — small software consultancy I run
- Kernel email: `loukot@gmail.com` — attribution for [my lore.kernel.org posts](https://lore.kernel.org/all/?q=f:loukot@gmail.com)

---

<sub>If my open source work has been useful to you, consider supporting it via [Ko-fi](https://ko-fi.com/prolificstudio) or [Buy Me a Coffee](https://buymeacoffee.com/prolificdev) ☕</sub>
