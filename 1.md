VB.NET
Write a Vb.net program for blinking an image
Program:- 
Public Class slip2

    Private Sub Timer1_Tick(sender As Object, e As EventArgs) Handles Timer1.Tick

        PictureBox1.Visible = Not PictureBox1.Visible

    End Sub

End Class

Design:- 

1) Get  Picturbox and timer control on design form.

2) Make timer control Enabled=True 

3) Insert image on Picturebox 

4) To fit the image PictureBox set Sizemode property to StretchImage
...............///////////.........../////////........///////////.......//////////


