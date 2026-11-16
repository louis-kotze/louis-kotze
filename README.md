### Hi, I'm Louis 👋

Senior full stack engineer based in South Africa. I build enterprise web applications by day and spend a fair bit of my spare time fixing the Linux Wi-Fi stack, which started when my own hardware misbehaved.

**Personal site + writing:** [louiskotze.dev](https://louiskotze.dev)

#### Open source work

Mostly the Linux Wi-Fi stack: over 20 commits merged across five projects since April 2026.

- **[wpa_supplicant / hostap](https://git.w1.fi/cgit/hostap/log/?qt=author&q=Kotze)**: fixed four bugs I reproduced on Wi-Fi 7 access points: stale per-link scan entries and per-link key clearing in multi-link (MLO) handling, duplicated elements in the Association Request, and falling back from PMKSA caching when the AP deauthenticates. Two came with new hwsim regression tests; all four shipped in wpa_supplicant 2.12. I later added a Multi-Link element fuzzer to the test suite. It found a one-byte over-read reachable before authentication from a crafted beacon (low severity), which I fixed in the same series (merged October 2026, after 2.12).
- **[Linux kernel](https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git/log/?qt=author&q=Louis+Kotze)**: an rtw89 fix for RF-calibration timeouts on USB adapters (mainline since 7.2, tested on four Realtek USB chipsets), and cfg80211 error messages that say why the BSS lookup for an authentication or association failed, with KUnit tests (mainline since 7.3).
- **[NetworkManager MR !2405](https://gitlab.freedesktop.org/NetworkManager/NetworkManager/-/merge_requests/2405)**, merged July 2026: NetworkManager reads the AP-MLD address from the Multi-Link element and, when every BSSID seen belongs to one Wi-Fi 7 access point, uses the long background-scan interval instead of the default five-minute one.
- **[wireless-regdb](https://git.kernel.org/pub/scm/linux/kernel/git/wens/wireless-regdb.git/log/?qt=author&q=Kotze)**: updates for South Africa, Hong Kong, Russia, South Korea, Ukraine and Togo, each checked against the primary source: the national regulator's published rules, or for Ukraine's 60 GHz entry, ETSI EN 302 567. Also a `Reviewed-by` on another contributor's Russia 6 GHz patch.
- **[morrownr/rtw89 PR #76](https://github.com/morrownr/rtw89/pull/76)**, merged April 2026: the RF-calibration fix backported to the out-of-tree DKMS driver.

#### Elsewhere

- [louiskotze.dev](https://louiskotze.dev) — personal site, blog, and CV downloads
- [Prolific Studio](https://prolificstudio.co.za) — small software consultancy I run
- Kernel email: `loukot@gmail.com` — attribution for [my lore.kernel.org posts](https://lore.kernel.org/all/?q=f:loukot@gmail.com)

---

<sub>If my open source work has been useful to you, consider supporting it via [Ko-fi](https://ko-fi.com/prolificstudio) or [Buy Me a Coffee](https://buymeacoffee.com/prolificdev) ☕</sub>
