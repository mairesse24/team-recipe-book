# Instructions to Fix Your Recipe Book Project

## Critical Issues to Address

Your recipe book implementation is **mostly complete and functional**, but there are a few important issues that need fixing:

### Issue 1: Wrong README Content (CRITICAL)
**Problem:** Your README.md file describes a "Driver Buddy" carpooling app instead of your recipe book project.

**Fix:**
1. Open `README.md` in your code editor
2. Delete ALL current content
3. Replace with:

```markdown
# Team Recipe Book 🍴

A collaborative recipe book created by our team to share favorite recipes and learn Git/GitHub!

## Team Members
- **Mairesse Nkundizanye** - Summer Travel Plans
- **Aasmi Joshi** - Nepali Momo Recipe
- **Madiha Syeda** - Chocolate Chip Cookies
- **Aavash Adhikari** - Fluffy Pancakes

## Recipes Included
- 🥗 Mairesse's Summer Plan
- 🥟 Aasmi's Nepali Momo
- 🍪 Madiha's Chocolate Chip Cookies
- 🥞 Aavash's Fluffy Pancakes

## How to View
1. Clone this repository
2. Open `index.html` in your web browser
3. Navigate through our recipes and about page

## Technologies Used
- HTML5
- CSS3 (Embedded styling)
- Git & GitHub for collaboration

## Project Purpose
This project was created as part of CSCE 1015 at UNT to practice:
- Team collaboration with Git
- HTML/CSS web development
- Version control and branching
- Creating a shared online resource
```

4. Save the file
5. Commit: `git add README.md`
6. Commit: `git commit -m "Fix README to describe recipe book project"`

---

### Issue 2: Duplicate README Files (CRITICAL)
**Problem:** You have both `readme.md` and `ReadMe.md` in your repository. This causes case-sensitivity issues.

**Fix:**
1. Run: `git rm ReadMe.md` (remove the duplicate)
2. Keep only `README.md` (all caps)
3. Commit: `git commit -m "Remove duplicate readme file"`

---

### Issue 3: Madiha's Recipe File Has Broken Image
**Problem:** In `madiha-recipe.html`, line 9 has image code but no actual image URL.

**Fix:**
1. Open `madiha-recipe.html`
2. Find line 9: `alt="Tasty choclate chip cookies"`
3. Replace with:
```html
<img src="https://images.unsplash.com/photo-1499636136210-6f4ee915583e?w=300"
     alt="Tasty chocolate chip cookies"
     width="300">
```
4. Save and commit: `git commit -am "Add image to Madiha's recipe"`

---

### Issue 4: Minor Spelling Errors
**Problem:** "choclate" appears multiple times instead of "chocolate"

**Fix:**
1. In `madiha-recipe.html`:
   - Line 7: Change "Tasty choclate chip cookies" to "Tasty chocolate chip cookies"
   - Line 9: Already fixed above
2. In `index.html` line 132:
   - Change "Madiha's choclate chip cookies" to "Madiha's chocolate chip cookies"
3. In `about.html` line 157:
   - Change "Madiha's choclate chip cookies" to "Madiha's chocolate chip cookies"
4. Commit: `git commit -am "Fix spelling of chocolate"`

---

## Team Contribution Summary

Based on git history (102 total commits):
- **Mairesse (mairesse24)**: 59 commits (58%) - Primary developer, created index/about pages, styling
- **Aasmi Joshi**: 20 commits (20%) - Created Momo recipe, contributed to about page
- **aasjos**: 9 commits (9%) - Same person as Aasmi (different account)
- **Aavash (aavashrzx)**: 8 commits (8%) - Created pancake recipe
- **Madiha (madiha4558)**: 6 commits (6%) - Created cookie recipe

**Note:** Aasmi has two GitHub accounts being used. Should consolidate to one account.

---

## What's Working Well ✅

Your project has several strengths:
1. **Professional styling** - Beautiful color scheme and hover effects
2. **Complete navigation** - Home and About pages work perfectly
3. **All recipes present** - 4 complete recipe files
4. **Consistent design** - Unified look across all pages
5. **Responsive layout** - Centered containers and proper spacing

---

## Next Steps

1. Fix the README.md content (Issue 1) - **5 minutes**
2. Remove duplicate readme file (Issue 2) - **2 minutes**
3. Add missing image to Madiha's recipe (Issue 3) - **3 minutes**
4. Fix spelling errors (Issue 4) - **5 minutes**
5. Push all changes to GitHub
6. Verify on GitHub that README displays correctly

**Total estimated time: 15-20 minutes**

---

## How to Submit Fixes

After making all changes:

```bash
git add .
git commit -m "Fix README, remove duplicates, add image, fix spelling"
git push origin main
```

Then verify on GitHub that:
- README shows recipe book information (not Driver Buddy)
- Only one README.md file exists
- Madiha's recipe shows a cookie image
- All spelling is correct

---

## Questions?

If you encounter any issues while fixing:
1. Check that you're in the correct directory
2. Make sure you have the latest code: `git pull origin main`
3. Verify changes before committing: `git status`
4. Test the website locally by opening `index.html` in a browser

Good luck! Your recipe book is almost perfect - just needs these quick fixes!
