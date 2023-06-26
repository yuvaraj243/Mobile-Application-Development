# Ex.No: 2 To develop an application that uses GUI Components with Fonts and Colors. 


## AIM:

To create an application that uses GUI Components with Fonts and Colors using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:
Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next.

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.


## PROGRAM:
Program to print the text “GUIcomponent”.
## Activity_main.xml:
<?xml version="1.0" encoding="utf-8"?>

<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"

xmlns:app="http://schemas.android.com/apk/res-auto"                                                                                     

xmlns:tools="http://schemas.android.com/tools"    

android:layout_width="match_parent"

android:layout_height="match_parent"    

tools:context=".MainActivity">
    

    <Button   
        android:id="@+id/colorButton"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_centerHorizontal="true"
        android:layout_marginStart="120dp"
        android:text="Change Color"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/fontButton"
        app:layout_constraintVertical_bias="0.082" />

    <Button
        android:id="@+id/fontButton"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_below="@id/colorButton"
        android:layout_centerHorizontal="true"
        android:layout_marginStart="120dp"
        android:layout_marginTop="120dp"
        android:text="Change Font"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/textView" />

    <TextView
        android:id="@+id/textView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_below="@id/fontButton"
        android:layout_centerHorizontal="true"
        android:text="Hello World!"
        android:textSize="40sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.435"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.325" />

</androidx.constraintlayout.widget.ConstraintLayout>

## MainActivity.java:
package com.example.myapplication;

import androidx.appcompat.app.AppCompatActivity;

import android.graphics.Color;

import android.graphics.Typeface;

import android.os.Bundle;

import android.view.View;

import android.widget.Button;

import android.widget.TextView;

public class MainActivity extends AppCompatActivity {

    private Button colorButton;
    
    private Button fontButton;
    
    private TextView textView;
    
    @Override
    
    protected void onCreate(Bundle savedInstanceState) {
    
        super.onCreate(savedInstanceState);
        
        setContentView(R.layout.activity_main);
        
        colorButton = findViewById(R.id.colorButton);
        
        fontButton = findViewById(R.id.fontButton);
        
        textView = findViewById(R.id.textView);
        
        colorButton.setOnClickListener(new View.OnClickListener() {
        
            @Override
            
            public void onClick(View v) {
            
                changeTextColor();
                
            } });

        fontButton.setOnClickListener(new View.OnClickListener() {
        
            @Override
            
            public void onClick(View v) {
            
                changeFont();
                
            }
        });
    }
    private void changeTextColor() {
    
        int randomColor = Color.rgb(
        
                (int) (Math.random() * 256),
                
                (int) (Math.random() * 256),
                
                (int) (Math.random() * 256)
        );
        textView.setTextColor(randomColor);
    }
    private void changeFont() {
    
        Typeface[] fontStyles = new Typeface[]{
        
                Typeface.DEFAULT,
                
                Typeface.DEFAULT_BOLD,
                
                Typeface.MONOSPACE,
                
                Typeface.SANS_SERIF,
                
                Typeface.SERIF
                
        };

        int randomIndex = (int) (Math.random() * fontStyles.length);
        Typeface selectedFont = fontStyles[randomIndex];
        textView.setTypeface(selectedFont);}
   }


Developed by: Rajavarman P

Registeration Number : 212220220032


## OUTPUT
![Screenshot (186)](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/91f48800-f52b-485c-8052-a0b20e569ff1)

![Screenshot (187)](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/2a80aa27-705c-4b88-a9d2-1c759c33d270)

![Screenshot (189)](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/a0736a91-1e7c-4be5-9410-6c258e0f0d82)

![Screenshot (190)](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/595b41c7-0317-4e7d-94a2-6881fa40bd0f)

![ex2 1](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/4ca4dc6d-5c97-40c7-8265-c2610651407a)


![ex2 3](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/0897f74b-73c4-4267-9b2f-f58b63bbbd64)



## RESULT
Thus a Simple Android Application that uses GUI Components with Fonts and Colors using Android Studio is developed and executed successfully.


