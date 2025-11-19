# unsafe-search-blocklist
DNS Blocklist for unsafe search sites

# AdGuard Home Blocklist: Unsafe Search, Shopping, and AI

This blocklist is designed to **supplement** SafeSearch enforcement and DNS-based blocking (e.g., via AdGuard Home, Pi-hole, or OpenDNS). It targets platforms where minors might still encounter **adult, harmful, or unmoderated content**—even with SafeSearch enabled—such as:

- **Image/video search results** on search engines without forced SafeSearch.
- **Shopping sites** known for selling adult or unsafe products.
- **AI platforms** generating unmoderated or explicit content.

## Why Use This List?
- **SafeSearch is not foolproof**: Some search engines (e.g., Brave) allow adult content in image/video results unless manually restricted.
- **Shopping/AI risks**: Many sites show adult content without age verification.
- **Layered protection**: Use this alongside SafeSearch enforcement and DNS filtering for comprehensive safety.

## Usage
1. Add the raw blocklist URL to AdGuard Home:
https://raw.githubusercontent.com/brtz2001/unsafe-search-blocklist/main/unsafe-search-blocklist.txt
2. Ensure SafeSearch is enforced via DNS or admin settings for e.g. Google/Bing.
3. Combine with other blocklists (e.g., [Hagezi’s DNS Blocklists](https://github.com/hagezi/dns-blocklists)) for broader coverage.

## How This List Was Generated

This blocklist was generated using the following prompt, designed to ensure comprehensive protection for minors by targeting search engines, shopping sites, and AI platforms that do not enforce safe content by default:

---
Generate an updated **plain domain blocklist** for protecting minors, as of today’s date. Follow these rules:

**1. Block all search engines that do NOT enforce safe search by default** (except Google, assuming SafeSearch is enforced via admin/DNS).
   - Include: DuckDuckGo, Brave, Yahoo, Bing, Yandex, and all others without forced safe search.

**2. Block all shopping sites notorious for unsafe, scammy, or adult content.**

**3. Block all AI platforms known for unmoderated, adult, or harmful content.**

**4. Requirements:**
   - Format as a **plain domain list**, one domain per line.
   - **Comments are allowed** to separate categories (e.g., `# Search Engines`).
   - **No need to remove defunct domains**—keep them for historical/reference purposes.
   - Example format:
     ```
     # Search Engines Without Forced Safe Search
     duckduckgo.com
     search.brave.com
     search.yahoo.com
     ```
   - Current list: https://raw.githubusercontent.com/brtz2001/unsafe-search-blocklist/main/unsafe-search-blocklist.txt
     
**5. Output only the commented plain domain list, nothing else.**
          
---

## About This List
This blocklist was **generated with the assistance of an AI tool** based on human-curated criteria for protecting minors online. The list is a **functional compilation of publicly available domain names** and is provided as-is under the [Creative Commons Zero (CC0)](LICENSE).

- **No copyright is claimed** over the individual domains.
- **You are free** to use, modify, and share this list under the terms of the license.

## License
This blocklist is dedicated to the **public domain** using [Creative Commons Zero (CC0)](LICENSE). You are free to use, modify, and distribute it for any purpose, without restrictions.

