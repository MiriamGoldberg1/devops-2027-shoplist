# pytho גרסה 3.11 ב   
FROM python:3.11-slim

# העתקת קובץ התלויות לפני הקוד, כדי ששלב ההתקנה יישמר ב-cache
COPY requirements.txt

# התקנת התלויות ללא שמירת קבצי התקנה זמניים
RUN pip install --no-cache-dir -r requirements.txt

# העתקת קוד השרת לתוך ה-image
COPY app.py .

#  הפורט שהשרת מאזין עליו
EXPOSE 8000

#  הפעלת השרת ע"י שורת הפקודה שנארזה פה גם 
CMD ["python", "app.py"]
