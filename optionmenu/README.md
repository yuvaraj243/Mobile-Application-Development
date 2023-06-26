# Ex.No:10 To create a option menu to display menu items.


## AIM:

To create a option menu to display menu items using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:
Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as optionmenu and click Next.

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout using UI components in activity_main.xml.

Step 6: Display the calculator operation in MainActivity file.

Step 7: Save and run the application.


## PROGRAM:
Program to print the text “optionmenu”.

## Activity_main.xml:
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
              
    xmlns:tools="http://schemas.android.com/tools"
              
    android:layout_width="match_parent"
              
    android:layout_height="match_parent"
              
    android:orientation="vertical"
              
    android:padding="16dp"
              
    tools:context=".MainActivity">

    <TextView
        android:id="@+id/messageTextView"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="Select an option from the menu"
        android:textSize="25dp" />

</LinearLayout>

## MainActivity.java:
package com.example.optionmenu;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;

import android.view.Menu;

import android.view.MenuItem;

import android.widget.TextView;

import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    private TextView messageTextView;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
    
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        messageTextView = findViewById(R.id.messageTextView);
    }

    @Override
    public boolean onCreateOptionsMenu(Menu menu) {
    
        getMenuInflater().inflate(R.menu.options_menu, menu);
        return true;
    }

    @Override
    public boolean onOptionsItemSelected(MenuItem item) {
        int itemId = item.getItemId();

        switch (itemId) {
            case R.id.menu_item_1:
                messageTextView.setText("Option 1 selected");
                return true;
            case R.id.menu_item_2:
                messageTextView.setText("Option 2 selected");
                return true;
            case R.id.menu_item_3:
                messageTextView.setText("Option 3 selected");
                return true;
            default:
                return super.onOptionsItemSelected(item);
        }
    }
}

## Option_View.xml:
<menu xmlns:android="http://schemas.android.com/apk/res/android">
  
    <item
        android:id="@+id/menu_item_1"
        android:title="Option 1"
        android:textSize="25dp"/>
    <item
        android:id="@+id/menu_item_2"
        android:title="Option 2"
        android:textSize="25dp"/>
    <item
        android:id="@+id/menu_item_3"
        android:title="Option 3"
        android:textSize="25dp"/>
</menu>


Developed by: Rajavarman P

Registeration Number : 212220220032


## OUTPUT
![Screenshot (261)](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/aa05cad2-b27f-4bf5-a633-3ab2cb224ab1)

![Screenshot (262)](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/757ed84a-b1d2-449b-b3a2-86c45e3d9942)

![Screenshot (264)](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/7ea58072-0c2b-4e48-b290-118e771619bd)

![ex10 1](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/b4a29918-e08b-4967-829c-a25dd874f649)

![ex10 2](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/2d688bd5-39a1-4159-803e-b15e7bee7e87)

![ex10 3](https://github.com/Aishwarya-TM/Mobile-Application-Development/assets/127846109/9d7193ed-d934-4208-9fbb-db1614fd53d8)


## RESULT
Thus a Simple Android Application to create a option menu to display menu items using Android Studio is developed and executed successfully.


