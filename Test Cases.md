## Test Cases – Mentors Module

---

### TC-01 – Mentors tab visibility

## Environment
- Application: FC Learning Portal  
- URL: https://mentor.futurecollars.test.lncd.pl/  
- Browser: Chrome  
- OS: Windows 11  
- Test credentials:
  - Username: test_user  
  - Password: test_password  

**Preconditions:** User is logged in  

**Priority:** 1

**Steps:**
1. Open “Mentors” tab from dashboard  
2. Observe course tabs  

**Expected Result:**
- Mentors page opens successfully  
- Multiple course tabs are visible  
- Default tab “0Strawberries” is selected  
- Mentors list is empty  

---

### TC-02 – Tab interaction

## Environment
- Application: FC Learning Portal  
- URL: https://mentor.futurecollars.test.lncd.pl/  
- Browser: Chrome  
- OS: Windows 11  
- Test credentials:
  - Username: test_user  
  - Password: test_password  

**Preconditions:** Mentors page is visible and loads correctly (Test TC-01) 

**Priority:** 1

**Steps:**

1. Call Test: TC-01 – Mentors tab visibility validation  
   → Mentors page is loaded and course tabs are visible
2. Click on "Frontend" tab  
   - Expected Result: "Frontend" tab becomes active and mentors list is displayed  

3. Click on "Data Science" tab  
   - Expected Result: Tab becomes active, mentors list is displayed, "Duty hours" section is visible  

4. Click on "0Strawberries" tab  
   - Expected Result: Tab becomes active and mentors list is empty  

**Expected Result:**
- Tabs switch correctly  
- Each tab displays correct mentor data  
- Default tab shows empty state  

---

### TC-03 – Duties functionality

## Environment
- Application: FC Learning Portal  
- URL: https://mentor.futurecollars.test.lncd.pl/  
- Browser: Chrome  
- OS: Windows 11  
- Test credentials:
  - Username: test_user  
  - Password: test_password  

**Preconditions:** Mentors page is visible and loads correctly (Test TC-01)  

**Priority:** 1

**Steps:**

1. Call Test: TC-01 – Mentors tab visibility validation  
   → Mentors page is loaded and course tabs are visible  

2. Click on "Data Science" tab  
   - Expected Result: Mentors list is displayed, "Duty section" and "Add a duty" button are visible  

3. Select mentor "Jan Garstecki"  
   - Expected Result: Duties section updates and "Add a duty" button becomes active  

4. Click "Add a duty" button  
   - Expected Result: "Add a duty" form is displayed  

5. Select "Day of the week" → Monday  
   - Expected Result: Field accepts input  

6. Select "Start time" from the drop down menu → 03:30  
   - Expected Result: Field accepts input  

7. Select "Duration" from the drop down menu → 0:30  
   - Expected Result: Field accepts input  

8. Click "Save" button  
   - Expected Result:
   - Duty is created successfully  
   - Duty appears in list  
   - Correct day, time, and duration are displayed  
