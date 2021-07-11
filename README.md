# Easy-Permissions-in-Android
Implementing Easy Permissions in Android



####  Project Creation and adding the dependency
Open the Android Studio and create a project with Empty Activity template.

After creating the project, our next step is to add the dependency of EasyPermissions in our app level build.gradle file. Add the below line in the build.gradle file to have the dependency of EasyPermissions and after that sync your project.

// For developers using AndroidX in their applications
implementation 'pub.devrel:easypermissions:3.0.0'
 
// For developers using the Android Support Library
implementation 'pub.devrel:easypermissions:2.0.1'


#### Adding Permission in AndroiManifest.xml file
In order to take Dangerous Permission in our application, we have to display an alert to ask for permission. So, these permissions must be added in the AndroidManifest.xml file. By doing so, if the permission is granted by the user, the app can use that permission. Add the below lines:

<uses-permission android:name="android.permission.CAMERA" />
<uses-permission android:name="android.permission.ACCESS_FINE_LOCATION" />
<uses-permission android:name="android.permission.READ_SMS" />
<uses-permission android:name="android.permission.READ_CONTACTS" />
