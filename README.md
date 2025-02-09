# AntiMagiskRootDetection
 Avoid Magisk root detection 

- Install Magisk Alpha from https://t.me/magiskalpha
- Hide Magisk by installing the proxy app and change the default "Settings" name to something different
- Disable the built-in Zygisk of Magisk
- Make sure "Enforce denylist" is NOT enabled
- Install these Magisk modules:
    * https://github.com/LSPosed/LSPosed.github.io/releases (IMPORTANT: Shamiko doesn't have automated updates, so its your responsibility to keep it up to date otherwise the root hiding will fail with security updates)
    * https://github.com/Dr-TSNG/ZygiskNext
    * https://github.com/chiteroman/PlayIntegrityFix
- Reboot
- Open the Magisk app and go to Modules, then tap the "Action" button below the "PlayIntegrityFix" module to pull a fingerprint
- Clear the cache of Google Play Services
- Reboot
- Re-install the detected apps and add them to the denylist before launching them

Magisk Alpha is a well maintained fork, but Magisk Canary or Magisk Delta (Kitsune) may also work. ZygiskNext is most importantly required.

## Feb. 2025 Update

With a recent change to the Google Play integrity system (especially for Android 13+), more apps started detecting root.

It seems to be fixed by installing a Magisk module called TrickyStore (this was also recommended by the Magisk Alpha dev on their Telegram channel)

You need TrickyStore alongside Play Integrity fix. See https://github.com/chiteroman/PlayIntegrityFix/releases/tag/v18.5

TrickyStore can be found at https://github.com/5ec1cff/TrickyStore

You can also check https://www.reddit.com/r/Magisk/comments/1gegtr4/tutorial_using_trickystore_with_zygisk_next_for/ for a tutorial (but ignore the part that says "remove PlayIntegrityFix to avoid conflicts")

## Also,

It seems that the PIF/fingerprints served with the PlayIntegrityFix module now get banned way faster than before (although the dev of the module actively updates the fingerprints).

The best thing that can be done is to get your own fingerprint file, or to use one of the projects that automate pulling a fingerprint to avoid these bans.

* To get your own fingerprint file, see: https://xdaforums.com/t/module-play-integrity-fix-safetynet-fix.4607985/page-177#post-89189572
* For automated fingerprint pulling: 
  - https://github.com/daboynb/PlayIntegrityNEXT / https://github.com/daboynb/playcurlNEXT (easier to use)
  - https://github.com/osm0sis/PlayIntegrityFork?tab=readme-ov-file#about-autopif2sh-and-killpish-script-files (see https://xdaforums.com/t/module-play-integrity-fix-safetynet-fix.4607985/page-387#post-89233630 for a tutorial from the author)

Use https://play.google.com/store/apps/details?id=gr.nikolasspyr.integritycheck&hl=en to check the integrity (it's okay if you're unable to pass the STRONG_INTEGRITY check).

Make sure to add the Play Integrity API Checker app in your Magisk Denylist

IMPORTANT: Make sure your Shamiko is up to date. Remember that Shamiko doesn't have automated updates, so its your responsibility to keep it up to date. Check https://github.com/LSPosed/LSPosed.github.io/releases

## Thanks to
- https://fmhy.net/android-iosguide#root-flash
- https://awesome-android-root.link/apps#hide-root
- https://www.reddit.com/r/Magisk/comments/18tzkg4/comment/kfin1gx/
- https://xdaforums.com/t/module-play-integrity-fix-safetynet-fix.4607985/page-177#post-89189572
- https://xdaforums.com/t/module-play-integrity-fix-safetynet-fix.4607985/page-387#post-89233630
- https://www.reddit.com/r/Magisk/comments/18nqht2/news_new_play_integrity_fix_fork_is_awesome/
- https://xdaforums.com/t/instapay-banking-app-detects-root-help-please.4449849/post-89552360

## Official Telegram groups
- PlayIntegrityFix -> https://t.me/playintegrityfix
- playcurlNEXT -> https://t.me/playfixnext
- Magisk Alpha -> https://t.me/magiskalpha
