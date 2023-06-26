# Ex.No:1 To create a HelloWorld Activity using all lifecycles methods to display messages.


## AIM:

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

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
Program to print the text “Hello World”.
## Activity_main.xml:
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
    
    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:textSize="40dp"
        android:text="Hello World!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>

## MainActivity.java:
package com.example.myapplication;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(), "onCreate Called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onStart() {
        super.onStart();
        Toast toast = Toast.makeText(getApplicationContext(), "onStart Called", Toast.LENGTH_LONG);
        toast.show();
    }
    @Override
    protected void onRestart() {
        super.onRestart();
        Toast toast = Toast.makeText(getApplicationContext(), "onRestart Called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onPause() {
        super.onPause();
        Toast toast = Toast.makeText(getApplicationContext(), "onPause Called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onResume() {
        super.onResume();
        Toast toast = Toast.makeText(getApplicationContext(), "onResume Called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onStop() {
        super.onStop();
        Toast toast = Toast.makeText(getApplicationContext(), "onStop Called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onDestroy() {
        super.onDestroy();
        Toast toast = Toast.makeText(getApplicationContext(), "onDestroy Called", Toast.LENGTH_LONG);
        toast.show();
    }
}


Developed by: Rajavarman P

Registeration Number : 212220220032

## OUTPUT
![Screenshot (160)](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/7a58d5f9-c10c-4784-ae4d-3db065cac32b)


![Screenshot (163)](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/30be0111-0a2e-4b23-8e6a-3e5d63e31e3c)


![Screenshot (169)](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/74246c7e-4f82-43f2-b587-919cd7961d07)


![Screenshot (157)](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/91949c3a-a879-4109-a0e9-0bbef68091f6)


![Screenshot (156)](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/89b3631e-bfde-40a5-9b76-dce4f722f55e)


![Screenshot (159)](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/aea33167-b168-43a7-96c7-09d625711f25)


![Screenshot (164)](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/d23edc01-33fe-4307-af07-05a3fe5b4e2b)


![Screenshot (165)](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/f94ca89d-5b46-4e96-be7e-76733fb8966c)


![Screenshot (166)](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/60bba63d-3647-4d5e-a53f-55b37f2c3dd4)


![Screenshot (167)](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/970d2b11-7dd4-4c03-b3e0-d04066fb94e9)

 
 ![Screenshot (168)](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/f37ce849-4393-4218-a8a9-a18cb36f47b2)
 

![4](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/ba2c6654-e383-4126-be79-972260efe546)


![6](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/78ea5b3f-6f13-4e76-8009-fc3ace0b769d)


![5](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/19af6d19-722e-45f3-ba20-719a1065f768)


![2](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/506ef9e5-9425-4c4d-9b30-c761a2a521b6)


![1](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/4f4c2d00-8e2a-4fa5-b922-4300fe4477d7)


![3](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/c136b322-b093-49bf-af96-177f9979f782)

## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
