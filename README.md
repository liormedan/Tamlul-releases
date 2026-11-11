# Tamlul — הורדה

Tamlul היא תוכנת תמלול עברית ל-Windows. התמלול, העריכה והייצוא רצים כולם במחשב שלך: קבצי הווידאו, האודיו והתמלולים לא עולים לשום שרת.

הריפו הזה מכיל רק את קבצי ההתקנה. קוד המקור לא נמצא כאן.

## הורדה

הגרסה האחרונה נמצאת בדף **[Releases](../../releases/latest)**. מורידים את הקובץ `Tamlul_<גרסה>_x64-setup.exe` ומריצים אותו.

גרסאות שמסומנות **Pre-release** הן גרסאות בטא.

## דרישות מערכת

| | |
|---|---|
| מערכת הפעלה | Windows 10 או 11, ‏64 ביט |
| מקום פנוי | כ-12GB בזמן ההתקנה, כ-7GB אחריה |
| זיכרון | 8GB לפחות, 16GB מומלץ |
| כרטיס מסך | NVIDIA מומלץ. בלי כרטיס כזה התמלול רץ על המעבד, לאט יותר |
| אינטרנט | נדרש בהפעלה הראשונה בלבד |

## התקנה

1. מריצים את קובץ ההתקנה. ההתקנה היא למשתמש הנוכחי ולא דורשת הרשאות מנהל.
2. **אזהרת Windows SmartScreen:** קובץ ההתקנה עדיין לא חתום, ולכן Windows עשוי להציג "Windows protected your PC". לוחצים **More info** ואז **Run anyway**.
3. בהפעלה הראשונה נפתח אשף שמוריד את מנוע התמלול והמודלים (כ-5GB). זה לוקח בין 15 ל-40 דקות, לפי מהירות החיבור. ההורדה קורית פעם אחת בלבד.

## בדיקת הקובץ

לכל גרסה מצורף `SHA256SUMS.txt`. כדי לוודא שהקובץ שהורדת שלם:

```powershell
Get-FileHash .\Tamlul_<גרסה>_x64-setup.exe -Algorithm SHA256
```

הערך צריך להיות זהה לזה שבקובץ.

## הסרה

דרך "הגדרות ← אפליקציות" ב-Windows. הפרויקטים שלך נמחקים רק אם מסמנים במפורש את האפשרות למחוק גם אותם.

---

# Tamlul — downloads

Tamlul is a Hebrew transcription app for Windows. Transcription, editing and export all run on your own computer; your video, audio and transcripts are never uploaded.

This repository only hosts the installers. Download `Tamlul_<version>_x64-setup.exe` from **[Releases](../../releases/latest)**. Windows 10/11 64-bit; an NVIDIA graphics card is recommended. The installer is not code-signed yet, so SmartScreen may warn: choose **More info → Run anyway**. The first launch downloads the transcription engine and models (about 5GB) once. Each release includes `SHA256SUMS.txt` to verify the download.
