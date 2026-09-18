
---

### 💻 VISUAL BASIC 1 

**FILE 7: `Visual-Basic-1/Module-01.md`**
```md
# VB101 - Module 1: Your First Program

**What is Visual Basic?** Easy language to create Windows apps.

**Practical Steps:**
1. Install Visual Studio 2022
2. Create Project > Windows Forms App
3. Form Properties: Text = "IOB Calculator"
4. Toolbox: Add 2 TextBoxes, 1 Button, 1 Label

**Code for Button:**
```vb
Dim a As Integer = Val(TextBox1.Text)
Dim b As Integer = Val(TextBox2.Text)
Label1.Text = a + b

**FILE: `Visual-Basic-1/Module-02.md`**
```md

# Module 2: Forms, Controls & Logic

**Common Controls:**
- TextBox: Input
- Button: Click
- Label: Display
- ComboBox: Dropdown
- ListBox: List

**IF Statement Example - Grading System:**
```vb
Dim score As Integer = Val(txtScore.Text)
If score >= 80 Then
    lblGrade.Text = "A - Excellent"
ElseIf score >= 70 Then
    lblGrade.Text = "B - Very Good"
ElseIf score >= 60 Then
    lblGrade.Text = "C"
Else
    lblGrade.Text = "Fail"
End If

**FILE: `Visual-Basic-1/Module-03.md`**
```md

# Module 3: Connecting VB to Database (Oracle/Access)

**Steps to connect:**
1. Add Button "Save"
2. Import: Imports System.Data.OleDb
3. Code:
```vb
Dim conn As New OleDbConnection("Provider=MSDAORA;Data Source=XE;User ID=system;Password=oracle;")
conn.Open()
Dim cmd As New OleDbCommand("INSERT INTO Students VALUES(1,'Ama','IT')", conn)
cmd.ExecuteNonQuery()
MsgBox("Saved!")
conn.Close()
