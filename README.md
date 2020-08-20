# My_Notebook
Notebook android app for entering and saving notes. Ability to change layout theme to (Dark Theme) from drawer.
Database: RoomDB

minSdkVersion: API 21 android 5.0.0
targetSdkVersion: 29
buildToolVersion: 29.0.2

DATABASE: ROOM DATABASE

Used as a local backend database to perform the following tasks on user entered Notes:
-> Insert notes into Room DB
-> Retrieve notes from Room DB and display to user in RecyclerView.
-> Delete notes from Room DB/ delete user selected notes.
-> Update user selected notes in Room DB.

Application Interface:
-> Ability to share notes to 3rd party external applications(WhatsApp, Gmail, Instagram, Facebook, G-Drive etc).
-> Ability to switch between app theme (Dark Theme) from navigation drawer.

Required Dependencies: build.gradle(Module:app)
  //Room database
    implementation 'androidx.room:room-runtime:2.2.5'
    annotationProcessor 'androidx.room:room-compiler:2.2.5'
    implementation 'androidx.paging:paging-runtime:2.1.2'
    testImplementation 'androidx.room:room-testing:2.2.5'
    
    //Material Drawer
        implementation('com.mikepenz:materialdrawer:7.0.0@aar') {
            transitive = true
        }
