# Attendance_Face_Recognition

An Attendance system using Face Recognition

### Instructions

1. Add student face images in students folder.
2. Renname face images with roll no.
3. For example, roll no 1 image is saved as '1.jepg'

### Prerequisities

1. OpenCV
```
pip install opencv-python
```

1. Dlib
```
pip install dlib
```

2. Face Recognition
```
pip install face-recognition
```

### Implementation

1. Run the program
```
python3 attendance.py
```

2. This launches the webcam and starts detecting faces.
  -  If an unknown face is detected (not in students images folder) it labels them at 'Unknown'.
  -  If faces are identified, it displays their roll no in the label and logs in an Excel sheet.
  
3. Press 'q' on keyboard to stop the attendance process (closes the webcam)


4. The output is an excel sheet 'att_month_(current month no).xlsx'
  - So If it is January the file is 'att_month_1.xlsx'
  - If it is February the file is 'att_month_2.xlsx'

5. The attendance is then logged in columns as per the day.
 - So if it is Jan 5 it logs in column E
 - if it is Jan 2 it logs in column B

6. Then the faces whose roll nos were identified are marked as 'Present' in the respective row no (same as roll no)



