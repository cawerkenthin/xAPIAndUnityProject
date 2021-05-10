# xAPIAndUnityProject
Example of embedding xAPI in a Unity Project

This is an example of sending and querying xAPI statements in a Unity 3D project.  The game is based on Roll A Ball example from Learn.Unity.com.  The project uses the GBLXAPI.org library for unity.  The required files for GBLXAPI are included in the package, but you may wish to get the latest version from GBLXAPI.org.  This project was created for demonstration purposes and was not intended for production use.  For more information, see https://learningsolutionsmag.com/articles/use-the-gblxapi-library-to-send-xapi-statements-from-unity

To see this project in action, you must first get a license for Unity from Unity.com.  Once done and you have installed Unity, follow these steps.

1. Create a new Unity Universal Render Pipeline project.
2. Delete the Sample Scene from your project.
3. From the Unity Asset Store, download and import the following free assets:
   * Free Fantasy Adventure Music Pack from "Craze Music Productions"
   * Free Casual Game SFX from "Dustyroom"
   * Night Without Moon from "Stinky Toilet"  (Sorry, I did not make up the name)
4. In the Unity editor, go to Assets/Import Package/Custom Packager and import the RISC Roll A Ball.unitypackage.
5. Once imported, open "Start" scene.  You will be prompted import TMP Essentials and it is required.
6. Go to Window/Package Manager.  Install the "Input System" package from the Unity Registry. Answer Yes to the prompt. This will cause the Editor to restart.
7. Go to File/Build Settings. Add scenes Start, Level 1, Level 2, Leaderboard to "Scenes In Build".
8. Also in Build Settings, open Player Settings.
   * Set Architecture to x86_64.
   * In Other Settings, set Active Input Handing to "Both".  The editor will again restart.
9. Right click on the Assets/Scripts folder in the project and choose Open c# project.
10. Open Assets/GBLXAPI/Scripts/GBLConfig.cs. Provide your LRS Endpoint in LrsURL.
11. Open Assets/Scripts/GBL_Interface.cs.
    * Provide your lrs User value in lrsUser
    * Provide the lrs Password value in lrsPassword.
12. Back in the Unity Editor, with the "Start" scene still open, hit play!


