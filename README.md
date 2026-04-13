# social-sparks
package com.example.socialsparks


import android.annotation.SuppressLint
import android.app.ProgressDialog.show
import android.os.Bundle
import android.widget.Button
import android.widget.EditText
import android.widget.Toast
import androidx.activity.enableEdgeToEdge
import androidx.appcompat.app.AppCompatActivity
import androidx.core.text.set
import androidx.core.view.ViewCompat
import androidx.core.view.WindowInsetsCompat
import com.google.android.material.textfield.TextInputEditText
import com.google.android.material.textfield.TextInputLayout
import kotlin.TODO



class MainActivity : AppCompatActivity() {

    private fun run() {
        TODO("Not yet implemented")
    }

    @SuppressLint("MissingInflatedId", "SetTextI18n")
    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        enableEdgeToEdge()
        setContentView(R.layout.activity_main)

        val resultText = findViewById<EditText>(R.id.resultText)
        findViewById<Button>(R.id.resetButton)
        val suggestButton = findViewById<Button>(R.id.suggestButton)

        val timeInput = findViewById<TextInputEditText>(R.id.timeInput)


        suggestButton.setOnClickListener { }
        val time = timeInput.textDirection.toString().lowercase()

        if (time.isEmpty()) {
            Toast.makeText(this, "please enter time of day", Toast.LENGTH_SHORT).show
            return@SetOnClickListner
        }
        when (time) {
            "morning" -> "Send a good morning message "
            "afternoon" -> "Check in with a friend 😊"
            "evening" -> "Call a friend"
            else -> "Invalid input"

        }
        suggestButton.androidx.compose.foundation.layout.Column {

        }

        time == (("send good morning")


        /* resultText.setText(suggestion) */

                ("send good morning")).also { resultText.textDirection = it }


        //                           resultText.setText(suggestion)


//                            resultText.setText(suggestion)


//                            resultText.setText(suggestion)


//                            resultText.setText(suggestion)


        run()
        when (time) {
            "afternoon" -> {
                ("send good afternoon").also {
                    it.also { it: String -> resultText.text = it }
                }

            }
            else -> resultText.setText("Invalid Input")

        }

    }

}
