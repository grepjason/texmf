# romdev

## IAST Latin transliteration to Devanāgarī

**Changelog**:

2021-11-03 commented out lines 198-202 to make *aḥ* and *aṃ* work as expected.

2021-10-19 Updated `romdev.map` and `romdev.tec` to most recent versions. (See file header in `romdev.map` for details.)

2021-11-01 added *jihvamūlīya* and *upadhmanīya*.

2021-10-19 added the changes from urukrama at Github, adding

- the devanāgarī abbreviation sign and
- initial *aṃ*, *avagraha* and *anusvara* and *om* symbol (<https://github.com/somadeva/RomDev/pull/3>).

2014-07-26 added the following CC license, with explicit permission from Somdev Vasudeva:

    This work is licensed under the Creative Commons Attribution 4.0 International License. To view a copy of this license, visit <http://creativecommons.org/licenses/by/4.0/>.

v0.3. An improved version of my earlier TECkit map to dynamically convert UTF8 Romanized Sanskrit and Prakrit to Devanāgarī in XeLaTeX. This version fixes:

- Roman capitals are converted.
@@ -10,4 +15,4 @@ v0.3. An improved version of my earlier TECkit map to dynamically convert UTF8 R
- Support for Prakrit. You can use diaereses (gaa = gaä) and breves (only initial short e and o for now, e.g. ĕttha etc. ) and tildes to mark prosodically short nasalisations (e.g. tāĩ vs. tāiṃ or tāïṃ).
- Outstanding is support for Vedic accents.

The older file header from the version released on Somdev's [Sārasvataṃ Cakṣuḥ blog](https://web.archive.org/web/20101017085126/http://sarasvatam.blogspot.com/2010/03/updated-teckit-romdev.html), March 2010:

> An updated version of my earlier RomDev.map file that now supports Prakrit. You can use diaereses (gaa = gaä) and breves (only initial short e and o for now, e.g. ĕttha etc. ) and tildes to mark prosodically short nasalisations (e.g. tāĩ vs. tāiṃ or tāïṃ). TECkit mapping for Unicode romanised Skt. to DN conversion v0.2 Updated March 23, 2010 9:53:03 PM EDT
