Halloween 3.3.19
==============
For phpBB 3.3.19. Parent style: prosilver 3.3.19.
Style version: 3.3.19 (retained at the owner's request).
Updated: 2026-10-11.

DESIGN AND ATTRIBUTION
The 2026 refresh uses warm amber, compact title bars, orange form controls,
a lighter forum header and original SVG moonlight/forest/bat scenery.
The original Halloween logo, seasonal statistics artwork and forum/topic status
images are retained. Previous repeating backgrounds are optional originals
under contrib/original-artwork and are no longer loaded.
Based on prosilver by phpBB Limited and Tom Beddard. The supplied Halloween
header attributes its modifications to Onnozel Manneke; the supplied style
configuration/stylesheet credits SpIdErPiGgY. These credits are retained.
The footer author link is Halloween — Spiderpiggy Trivia,
https://spiderpiggy.com. Obsolete author-site links have been removed.
Style code is licensed under GPL version 2. See license.txt in this directory.
The archive contains no separate evidence of the original artwork licences or
transfer of authorship. These must be established before public submission;
including artwork here does not establish its ownership or permission.

INSTALL / UPDATE
1. Back up the complete existing styles/Halloween directory first.
2. Use the complete replacement Halloween directory supplied in this ZIP.
   Replace its contents, keeping the exact directory name and capitalisation.
   Do not mix old template/CSS files with the new package.
   An overwrite alone leaves obsolete files: remove the old root license.txt
   and contrib/Delete the bats.txt after confirming the backup exists.
   The licence is now at contrib/license.txt.
3. Keep prosilver installed and updated to 3.3.19. No extension or PHP edits
   are required. Existing Halloween style settings can remain installed.
4. ACP > General > Purge the cache. Hard-refresh the browser (Ctrl+F5).
5. New installation only: ACP > Customise > Install styles > Halloween.
6. Test your installed extensions and important forms on your own test board
   before deploying the replacement to the live board.

CUSTOMISATION
The shared phpBB layout CSS is included locally in theme/. The Halloween
layout/palette is in theme/halloween.css. Status icons and semantic colours
are in theme/colours.css. theme/stylesheet.css imports them in order.
UCP, MCP, searching, posting and other pages use current prosilver templates
through inheritance. Their common controls receive the Halloween palette.
Group and username colours are left under phpBB control.
To disable the decorative flying artwork, remove the INCLUDE bats.html line
from template/overall_header.html and purge the cache. No script is required.
It is already hidden on small screens and for reduced-motion preferences.

VALIDATION FIXES - 2026-10-11
The two reported denial issues are corrected. Isolated template fragments
were checked using conditional evaluation (not the phpBB/Twig runtime) for subforum URLs/read states/tooltips and all eight combinations
of forum description, moderators and MCP-link availability. This check is not
a new full-board validation. Earlier validation notes below are retained from
the supplied archive and were not independently repeated for this repair.

VALIDATION SCOPE (earlier supplied notes)
Header Banner 3.2.4 compatibility is automatic when the extension is enabled.
Its configured banner width, mobile image and search placement are preserved.
The extension itself does not need modification. Its original template output
and CSS were checked at seven viewport widths, including mobile and background
hiding options, as well as smaller centred banners.

Checked against the supplied phpBB 3.3.19 package and these policy references:
https://www.phpbb.com/styles/rules-and-policies/submission-policy/3.3/
https://www.phpbb.com/styles/rules-and-policies/submission-policy/3.1/
https://www.phpbb.com/styles/rules-and-policies/development-rules/
The 3.3 policy is the applicable submission reference. The 3.1 policy is
historical. Development rules also cover public topics/downloads, which
cannot be assessed from a ZIP archive.

All eight own templates compile using phpBB's bundled Twig engine on PHP 8.3.
All 129 upstream template-event occurrences and 21 named controls in the
seven upstream-based overrides match prosilver; form/hidden-token counts match.
The decorative bats template has no form controls or translation strings.
All 20 CSS files parse; local CSS imports/image references resolve.
All 67 supplied raster images verify successfully and retain their bytes
(including archived backgrounds/decorations); five original vector assets
parse.
Rendered index, signed-in navigation, UCP settings, MCP front page, search,
posting/BBCode preview, avatar-upload controls and RTL index fixtures were inspected in Chromium at
1280, 390 and 320 pixels. No horizontal page overflow in these 24 cases.
The eight fixture documents have no HTML5 parsing errors.
Count badges also centre on both axes at 1280, 900 and 701 pixels.
The avatar-delete checkbox toggles by keyboard; the upload button is amber. The phpBB credit is
present in each fixture; nickname inline colours remain unchanged.

These are isolated rendered fixtures, not a running database-backed board.
Posting, authentication, uploads and installed-extension integration still
require live-board testing. Firefox, Safari and legacy IE9 have not been
executed here. HTML/CSS parser checks are not W3C certification. Decorative
CSS may simplify in older browsers. Official Styles Team approval and
original artwork/redistribution permissions are not established by this check.
