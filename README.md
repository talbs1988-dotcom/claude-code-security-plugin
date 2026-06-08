# אבטחת סביבת Claude Code

מאבטח את Claude Code שלך ב-3 שכבות הגנה — בשיחה אחת.

## התקנה

העתיקי את ההודעה הזו לצ'אט Claude Code:

```
תתקין ותפעיל: https://github.com/talbs1988-dotcom/claude-code-security-plugin
```

זה מה שיקרה אוטומטית:

- ✅ חסימת קריאת קבצי `.env`
- ✅ Hook שחוסם `cat .env` בטרמינל
- ✅ כללי אבטחה ב-CLAUDE.md

## מה נבנה כאן

| שכבה            | מה                      | למה                                    |
| --------------- | ----------------------- | -------------------------------------- |
| Deny rules      | חוסם קריאת `.env`       | Claude לא יוכל לחשוף סודות גם אם יתבקש |
| PreToolUse hook | חוסם `cat .env` בפקודות | הגנה מפני prompt injection             |
| CLAUDE.md       | כללי התנהגות            | שכבת כוונה שמחזקת את ההגנות            |

---

בנוי על-ידי [טל בשור](https://talbs.co.il) לסדנת Claude Code.
