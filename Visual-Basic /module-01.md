
---

### 💻 VISUAL BASIC 1 - REMAINING

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
