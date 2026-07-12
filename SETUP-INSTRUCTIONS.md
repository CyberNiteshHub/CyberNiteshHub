# Setup Guide — GitHub Profile README

Ye folder tera **special profile repo** ban jayega. GitHub par jab kisi repo ka naam bilkul tere username jaisa hota hai (yahan `CyberNiteshHub`), toh uska README.md automatically tere profile page (github.com/CyberNiteshHub) par show hota hai.

## Steps

1. GitHub par ek naya repo banao — naam bilkul ye rakhna: `CyberNiteshHub` (tere username jaisa hi, case bhi match honi chahiye).
2. Repo **Public** rakhna aur README initialize mat karna (hum apna already-bana README use karenge).
3. Is poore folder (`README.md` + `assets/` wala) ko us repo me push kar do:

```bash
cd CyberNiteshHub-profile   # ye wahi extract ki hui folder hai
git init
git remote add origin https://github.com/CyberNiteshHub/CyberNiteshHub.git
git add .
git commit -m "Add profile README"
git branch -M main
git push -u origin main
```

4. Push hone ke 1-2 min baad apna profile (`github.com/CyberNiteshHub`) refresh karke check kar lena — card dikhne lagega.

## Files

- `README.md` — sirf card ko embed karta hai (`assets/profile-card.svg`).
- `assets/profile-card.svg` — poora terminal-style card (design, colors, layout tere image jaisa hi recreate kiya gaya hai — SVG hone ki wajah se GitHub par sharp/crisp render hoga aur zoom karne par bhi pixelate nahi hoga).
- `assets/ascii-portrait.txt` — card ke left panel wali ASCII art alag se, agar kabhi standalone chahiye ho.

## Customize karna ho toh

`assets/profile-card.svg` ek plain text file hai (SVG = XML). Kisi bhi text editor me khol ke:
- Numbers/stats (`Repos`, `Commits`, `Lines of Code` etc.) directly text me edit kar sakte ho.
- Colors `<defs>` aur har `fill="#..."` me hain, wahan se change ho sakte hain.
- Agar future me apna real photo se fresh ASCII portrait chahiye ho, mujhe naya photo bhejna — main dobara generate kar dunga.

Bas itna hi — direct push karo aur profile live ho jayega. 🚀
