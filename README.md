# Privacy Policy Repository

This repository hosts public privacy policy pages for my mobile applications using GitHub Pages.

---

## URLs and Deployment Status

| Type | Name | URL | Status / Use |
| --- | --- | --- | --- |
| Base GitHub Pages URL | Privacy Policy Repository | https://kartikhadiya09.github.io/privacy-policy/ | Main deployment for this repository |
| Privacy Policy | Money Radar | https://kartikhadiya09.github.io/privacy-policy/money-rader/ | Use this URL in app stores and app settings |
| Current app-ads.txt copy | Project app-ads.txt | https://kartikhadiya09.github.io/privacy-policy/app-ads.txt | Deployed from this repository, but not valid for AdMob verification |
| Required AdMob app-ads.txt | Root app-ads.txt | https://kartikhadiya09.github.io/app-ads.txt | Not deployed yet; this must be added to the `kartikhadiya09.github.io` repository root |
| Repository | GitHub Source | https://github.com/kartikhadiya09/privacy-policy | Source code repository |

---

## Important AdMob app-ads.txt Note

Google AdMob checks the `app-ads.txt` file only from the domain root.

The required root URL is currently expected to show `404 Not Found` until `app-ads.txt` is added to the `kartikhadiya09.github.io` repository root.

Required final URL:

```text
https://kartikhadiya09.github.io/app-ads.txt
```

Do not use this project-folder URL for AdMob verification:

```text
https://kartikhadiya09.github.io/privacy-policy/app-ads.txt
```

Because this repository is deployed under `/privacy-policy/`, an `app-ads.txt` file inside this repository becomes available at `/privacy-policy/app-ads.txt`. That URL is useful only as a copy/reference, but AdMob will not verify it from there.

To fix AdMob verification, create or update this file in the root of the `kartikhadiya09.github.io` repository:

```text
app-ads.txt
```

Current required content:

```text
google.com, pub-5419339606617664, DIRECT, f08c47fec0942fa0
```

After the root repository is updated, this URL should work:

```text
https://kartikhadiya09.github.io/app-ads.txt
```

---

## Repository Structure

```text
privacy-policy/
├── README.md
├── app-ads.txt
└── money-rader/
    └── index.html
```

---

## Notes

* Each app has its own folder.
* The `index.html` inside each folder acts as the public privacy policy page.
* All privacy policy pages are publicly accessible using GitHub Pages.
* AdMob `app-ads.txt` must be deployed at the root domain, not inside `/privacy-policy/`.
