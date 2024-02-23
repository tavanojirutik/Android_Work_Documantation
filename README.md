#table in AS
https://parallelcodes.com/android-how-to-scroll-listview-horizontally-and-vertically/

# Android_Work_Documantation

## Data and time Peacker
https://github.com/Pritish-git/date-and-time-picker-dialog/blob/main/MainActivity.java


##Select File in Android 

                    <Button
                    android:id="@+id/uploadAttachment"
                    android:layout_width="140dp"
                    android:layout_height="wrap_content"
                    android:text="Upload Attachment"
                    android:onClick="buttonOpenFile"
                    android:layout_marginStart="18dp"/>

Activaty_single_view_task.java

 //File Picker 
            private void openFilePicker() {
                Intent intent = new Intent(Intent.ACTION_GET_CONTENT);
                intent.setType("*/*"); // Set MIME type as "*/*" to allow any file type
                startActivityForResult(intent, PICK_FILE_REQUEST_CODE);
            }


            protected void onActivityResult(int requestCode, int resultCode, Intent data) {
                Activaty_single_view_task.super.onActivityResult(requestCode, resultCode, data);

                if (requestCode == PICK_FILE_REQUEST_CODE && resultCode == RESULT_OK) {
                    // Handle the selected file URI
                    Uri selectedFileUri = data.getData();
                    // TODO: Perform actions with the selected file URI
                }
            }
        });
