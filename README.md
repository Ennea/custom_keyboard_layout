The custom keyboard layout I use on my work PC. Modified US layout that swaps Z and Y and adds ä, Ä, ö, Ö, ü, Ü and ß to AltGr + A, O, U and S.

To use, move or copy `custom` into `/usr/share/X11/xkb/symbols`. Then edit `/usr/share/X11/xkb/rules/evdev.xml` and add the following XML at the end of the `<layoutList>` block:

```
<layout>
    <configItem>
        <name>custom</name>
        <shortDescription>encstm</shortDescription>
        <description>English (US, custom)</description>
        <languageList>
            <iso639Id>eng</iso639Id>
        </languageList>
    </configItem>
    <varianlist/>
</layout>
```
