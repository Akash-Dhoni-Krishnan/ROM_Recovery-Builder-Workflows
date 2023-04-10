# How to build Custom Recovery
| Supported Custom Recovery versions |
| -----------------------------------|
| Custom Recovery | Shorthand | Status | Note |
| TeamWin Recovery Project | `TWRP` | Fixing bugs |  |
| OrangeFox Recovery Project | `OFRP` | Fixing bugs |  |
| PitchBlack Recovery Project | `PBRP` |  | Coming soon |
| SkyHawk Recovery Project | `SHRP` |  | Coming soon |
- DON'T FORGET TO READ THE NOTES
## TeamWin Recovery Project
- According to the image, we have 9 lines that need to be filled in and edited
```bash
- Manifest Type
- Manifest Branch
- Device Tree URL
- Device Tree Branch
- Brand
- Device Code
- Makefile Type
- Add "export"
- Build Target
```
![😁Haha! I don't think your connection is too weak to see this picture 🤔🤔🤔](https://raw.githubusercontent.com/VThang51/Recovery-Builder-Workflows/main/images/Guide.png)
#### Manifest Type/Branch

- If your device uses Android 10+, use type "aosp". Otherwise use "omni" 

- Type and the corresponding Branch:
```bash
- omni
-- twrp-4.4-deprecated
-- ...
-- twrp-9.0
```
```bash
- aosp
-- twrp-11
-- twrp-12.1
```
#### Device Tree URL/Branch

- It's simply the URL and Branch of the Device Tree in your (or someone else's) Repository on GitHub 😋

#### Brand

- Your phone manufacturer

- Ex:
```bash
samsung
oppo
realme
```
- When filling in the Brand section, write all letters in lowercase

✅️
```bash
samsung
oppo
realme
```
❌️
```bash
Samsung
Oppo
Realme
```
#### Device Code/Makefile Type

- You can view it from the name of the .mk file

#### Add "export"

- This is used to fix build errors (You can leave it blank)

- If it fails during construction or needs an addition, follow the template below
```bash
export XXXXXX=1 && export YYYYYY=true && export ZZZZZZ=1
```
- Don't forget to add "&&"
#### Build Target

- Usually it will be "recovery", but in some cases it will be "boot"

## OrangeFox Recovery Project
- This line will be completed when I finish the file [OFRP.yml](https://github.com/VThang51/Recovery-Builder-Online/blob/main/.github/workflows/OFRP.yml)

## Note
- If you intend to develop this project, please clone this repository or submit a pull request.
- Thank you!!! 
