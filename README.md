# group26

At this point the master branch contains the starting stage of our android app

On our to do list:
1) Integrate camera api
2) Develop button press actions


// this code is of java for main window
package com.example.dawoodmehar.newwindowprc;

import android.content.Intent;
import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;
import android.view.View;
import android.widget.Button;

public class fir extends AppCompatActivity {

public Button but1;


public void  init(){
    but1=(Button)findViewById(R.id.jj);


    but1.setOnClickListener(new View.OnClickListener() {
        @Override
        public void onClick(View v) {
            Intent toy= new Intent(fir.this,Second.class);
        }
    });



}


// this code is for second window which i made from main window some thing is miss in tis i will let you know in 2 days
package com.example.dawoodmehar.newwindowprc;

import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;

public class Second extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_second);
    }
}



    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        init();
    }
}
