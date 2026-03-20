# סוכן חשבוניות — Gmail
ע
## הוראות הגדרה

### 1. הגדר את Google Client ID
פתח את הקובץ `public/index.html` וחפש את השורה:
```
const CLIENT_ID = 'GOOGLE_CLIENT_ID_HERE';
```
החלף את `GOOGLE_CLIENT_ID_HERE` ב-Client ID שלך מ-Google Cloud Console.

### 2. העלה ל-Vercel
1. כנס ל-vercel.com וצור חשבון חינמי
2. לחץ "Add New Project" ← "Upload"
3. גרור את תיקיית הפרויקט
4. לפני Deploy, הוסף Environment Variable:
   - Name: `ANTHROPIC_API_KEY`
   - Value: המפתח שלך מ-console.anthropic.com

### 3. הגדר Google Redirect URI
ב-Google Cloud Console, הוסף את כתובת ה-Vercel שלך כ-Authorized redirect URI:
```
https://YOUR-PROJECT.vercel.app
```

זהו! שלח את הקישור לעובדים שלך.
