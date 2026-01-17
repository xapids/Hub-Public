# Contact Generator - Quick Reference

**Fast lookup guide for when you're already set up.**

---

## 📱 Quick Workflow (iPhone)

1. **Open ChatGPT** → Tap "My GPTs" → "Contact Generator Assistant"
2. **Chat:** "Create contact for [name] at [company]"
3. **Answer questions** (3 at a time)
4. **Copy** the formatted data block
5. **Tap link** to open tool in Safari
6. **Paste** data → Tap "Parse & Fill"
7. **Review** → Tap "Generate & Download .vcf"
8. **Open** .vcf → Import to Contacts

**Total time: 1-2 minutes**

---

## 🖥️ Quick Workflow (Desktop)

Same as above, but use ChatGPT website instead of app.

---

## 🔗 Your URLs

**Web Tool (GitHub Pages):**
```
https://[your-username].github.io/contact-generator/contact-generator.html
```

**Custom GPT:**
- ChatGPT → "My GPTs" → "Contact Generator Assistant"

---

## 📋 Example Paste Data Format

```
contactType=Person
firstName=John
lastName=Smith
company=CleanHouse - Owner - Cleaner - Recommended by X - Self-Employed - 🇲🇹
phone1=+356 9999 8888
phone1Label=Mobile
email1=john@cleanhouse.com
email1Label=Email
url1=https://facebook.com/cleanhouse
url1Label=Facebook
birthday=15/03/1985
```

---

## ✅ Validation Checklist

Before generating .vcf:

- [ ] All phone numbers start with `+` (country code)
- [ ] All labels capitalized (Mobile, Email, Facebook, etc.)
- [ ] Company field has 5+ reference phrases (Person) or 4+ (Company)
- [ ] Country flag emoji at end of company field
- [ ] All URLs start with `https://`
- [ ] For companies: Google Maps link is direct (not search)
- [ ] For companies: First/Last name empty

---

## 🎨 Contact Types

### Person Contact:
- ✅ First Name (required)
- ✅ Last Name (if available)
- ✅ Company: min 5 phrases + flag
- ✅ Phone/Email/URLs (if available)
- ✅ Birthday (if available)
- ✅ Social profiles (if available)

**Example Company Field:**
```
CleanHouse - Owner - Cleaner - Recommended by X - Self-Employed - Mother of Y - 🇲🇹
```

### Company Contact:
- ❌ First Name (leave empty)
- ❌ Last Name (leave empty)
- ✅ Company: full name + min 4 phrases + flag
- ✅ Phone/Email/URLs (required: website + Google Maps)
- ❌ Birthday (leave empty)
- ❌ Social profiles (use URLs instead)

**Example Company Field:**
```
CleanHouse Ltd. - Cleaning Services - Recommended by X - Service Provider - Based in Valletta - 🇲🇹
```

---

## 🏷️ Common Labels

**Phone:**
- Mobile
- Landline
- Work
- Home

**Email:**
- Email
- Work
- Personal

**URL:**
- Website
- Facebook
- Instagram
- LinkedIn
- Google Maps
- Company

**Social:**
- Instagram
- LinkedIn
- Facebook
- X

**Always capitalize first letter!**

---

## 🌍 Country Code Examples

| Country | Code | Example |
|---------|------|---------|
| Malta | +356 | +356 9999 8888 |
| Germany | +49 | +49 170 1234567 |
| USA | +1 | +1 555 123 4567 |
| UK | +44 | +44 20 7123 4567 |
| Italy | +39 | +39 333 1234567 |
| Spain | +34 | +34 612 345 678 |

---

## 🚨 Common Errors & Fixes

### "Phone must start with country code"
**Fix:** Add `+356` or `+49` etc. before the number

### "URL must start with http://"
**Fix:** Add `https://` to the beginning

### "First Name is required"
**Fix:** You selected "Person" but didn't enter first name

### "Download didn't work"
**Fix:** Check browser permissions, try different browser

### "Google Maps link invalid"
**Fix:** Use direct business link, not search URL

---

## 🔧 Updating Your Custom GPT

If you need to change the web tool URL:

1. ChatGPT → "My GPTs" → "Contact Generator Assistant"
2. Click/tap "Edit GPT" (pencil icon)
3. Go to "Configure" tab
4. Find this line in Instructions:
   ```
   [Click here to open Contact Generator](URL_HERE)
   ```
5. Replace the URL
6. Click "Save"

---

## 📲 Add to iPhone Home Screen

**Make it like a native app:**

1. Safari → Open your tool URL
2. Tap **Share** button
3. Scroll → Tap **"Add to Home Screen"**
4. Name: "Contact Generator"
5. Tap **"Add"**

Now tap the icon anytime to launch!

---

## 🔄 Workflow Variations

### Skip ChatGPT (Fill Manually):
1. Open tool URL directly
2. Fill fields manually
3. Generate .vcf

**Good for:** Quick contacts, no ChatGPT Plus

### Use ChatGPT Without Custom GPT:
1. Regular ChatGPT chat
2. Ask: "Help me format a contact for John Smith"
3. Manually copy/organize data
4. Paste into tool

**Good for:** Free ChatGPT users

---

## 💡 Pro Tips

1. **Save common contacts as templates** in Notes
2. **Bookmark the tool** for instant access
3. **Keep country codes** in Notes for quick copy/paste
4. **Use ChatGPT to research** company info before creating contact
5. **Batch create contacts** - do multiple in one ChatGPT session

---

## 📁 File Locations

**On Your Computer:**
- `~/Desktop/contact-generator.html` - The web tool
- `~/Desktop/contact-generator-custom-gpt-instructions.md` - GPT setup
- `~/Desktop/SETUP-GUIDE.md` - Full setup instructions
- `~/Desktop/QUICK-REFERENCE.md` - This file

**Downloaded .vcf files:**
- `~/Downloads/[Name]_contact.vcf`

---

## 🆘 Quick Help

**Tool won't load:**
- Check internet connection
- Try different browser
- Clear browser cache

**Can't paste data:**
- Click in text box first
- Use keyboard shortcut (Cmd+V / Ctrl+V)

**Custom GPT not showing up:**
- Check you're in correct ChatGPT account
- Verify ChatGPT Plus subscription active

**Still stuck?**
- See SETUP-GUIDE.md for detailed troubleshooting
- Ask ChatGPT for help with error messages

---

**Happy contact creating! 📇✨**
