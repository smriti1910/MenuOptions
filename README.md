# Ex.No:10 To create a option menu to display menu items.


## AIM:

To create a option menu to display menu items using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:
```
Step 1: Open Android Studio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next.

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Create options.xml file under menu directory of res and write the code

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.
```


## PROGRAM:
```
/*
Program to print the text “optionmenu”.
Developed by:
Registeration Number :
*/
```
## activity_main.xml:
```
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
        android:text="Welcome Smriti!!!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>
```
## options.xml:
```
<?xml version="1.0" encoding="utf-8"?>
<menu xmlns:android="http://schemas.android.com/apk/res/android">
    <item android:title="Option 1" />
    <item android:title="Option 2" />
    <item android:title="Option 3" />
</menu>
```
## MainActivity.java:
```
package com.example.menu_options;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.view.Menu;
import android.view.MenuInflater;

public class MainActivity extends AppCompatActivity {
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }
    @Override
    public boolean onCreateOptionsMenu(Menu menu) {
        MenuInflater m = getMenuInflater();
        m.inflate(R.menu.options,menu);
        return true;
    }
}
```

## OUTPUT
![image](https://github.com/smriti1910/MenuOptions/assets/133334803/b4073ecd-7f90-4fa9-a25e-3ec484f3d5f7)
![image](https://github.com/smriti1910/MenuOptions/assets/133334803/f0b74a78-c5c6-4209-bee5-d1bdaaeebb4e)
![image](https://github.com/smriti1910/MenuOptions/assets/133334803/3b7dfc2a-bad3-41f0-8946-34952ae3251b)




## RESULT
Thus a Simple Android Application to create a option menu to display menu items using Android Studio is developed and executed successfully.

