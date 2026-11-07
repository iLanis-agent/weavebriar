# Weavebriar 1.0 TEST
Native Android Amibo equal-length bar-network puzzle. Android8+ (min26), target35. Package com.gg007.weavebriar.

## Rules
Amibo: form horizontal and vertical bars through cell centers, ending at cell borders. Each numbered circle must touch exactly one bar endpoint; the number gives that bar's length in cells, excluding the circle. Bars never pass through circles. Every bar must cross at least one bar of the SAME length, though it may also cross other lengths. All bars connect through crossings as one network with no closed loop. Bars without circles and empty cells are allowed. Neighboring collinear strokes merge into one bar. Tap each empty cell through blank, horizontal, vertical, cross and blank. Undo/reset/next/levels and saved weave palette/stroke marks. Twelve unique 4x3 circle layouts and unique solutions.

## Download and status
https://mega.co.nz/#!oBEzhTAL!4S1r4bW2mkal_wOYSrjK86XMfykgoBRPn8ixsaetHdA
APK SHA256 dde2cf485795cf1d5c3c560764b3d1cf50252f49abb15c732dc218750300a24e; 16878 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous download bytes match.

## Checks
Independent same-axis cell-component floodfill and graph-DFS oracle agrees with production maximal-run extraction and union-find validation on ALL3145728four-state freecell boards across12levels and120000invalid/random states. Each board has exactly one solution, with at least four bars. Circle layouts and cell-state solutions are all distinct. Actual archived segment-subset generator includes unanchored bars and reproduces levels.json; actual archived Java exhaustive tests pass. Invalid levels/arrays/values, circle lock, bounds, solved lock, solve/undo/replay/reset pass. Drawing-adapter four-state cycle/circle lock/undo, menu/settings/privacy/levels/next and saved preference/completion checks pass. Actual game/solved/menu/settings/privacy/levels drawing pixels inspected, not phone screenshots. Phone runtime, performance and external-browser handoff QA remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Live803-entry registry,125 recovered partial READMEs and semantic review of all151 prior studio cards found no Amibo match. Breezefen splits hub totals over uncrossed arms and covers every empty cell; Glowwillow connects turning firefly beams with turn counts. Weavebriar instead builds an acyclic crossing network of straight bars, each requiring an equal-length crossing partner, with optional unanchored bars and unused cells. Known Amibo genre published by Nikoli, not a global invention; recovered corpus is partial. Rules https://www.janko.at/Raetsel/Amibo/index.htm http://meanderlawn.blogspot.com/2016/02/amibo.html http://marshall.freeshell.org/nikoli_rules.html https://gamezipper.com/amibo/ https://playvori.com/g/amibo/ https://pzdc.blog.fc2.com/blog-entry-23.html .

## Build
JDK17 and AndroidSDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. Board.java embeds generated circle positions/numbers/solutions. javac -d /tmp/weave-test src/com/gg007/weavebriar/Board.java BoardTest.java and java -cp /tmp/weave-test com.gg007.weavebriar.BoardTest. bash build.sh creates an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to private original signing inputs. No credentials in source. Release build settings, signed TEST artifact, not final store release.

## Privacy and branding
Weavebriar runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Weave palette, stroke marks and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 icon byte-equal to original. Menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and websites
Complete source and APK privately preserved at https://files.instinct.com/xbtv9ufkbsv8-weavebriar-source-archive, including exact cumulative152-card studio and published catalog/studio sources/updater. Repository https://github.com/iLanis-agent/weavebriar holds README only; full Git source commit pending. Both website publications checked separately. No Pages settings change or Play rollout. November7,2026.
