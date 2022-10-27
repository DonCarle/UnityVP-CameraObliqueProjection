# UnityVP-CameraObliqueProjection
(Steps 1-2) if you don't already have SteamVr and this package in your project.
1. First download and import steamVR for unity: https://assetstore.unity.com/packages/tools/integration/steamvr-plugin-32647
2. Download and import the VirtualProductionCameraPackage.
3. In your scene pull in the VP prefab located in VP/Prefabs/OffaxisTracking_pf
4. Open the VP - Vp Camera setup window located in the menu bar. 
5. If you have the newest version VPTracker and OrientationManager should self assign. Else find them manually in the prefab and add them to the dedicated spots.
6. Measure and set the VP screen size in meters. 
7. If the tracker is far offset on the camera add the offset here also in meters.
8. If you haven't already make sure you tracker is enabled and tracking with steamVr.
9. Press play in unity and make sure the tracker is tracking. If it is attached and doesn't track select the VPTracker gameobject and change the index to Device 1, Device 2... etc to find which is tracking (NB. Also make sure you do this when you exit playmode as it will reset).
10. Take the tracker place it in the lower left corner of the screen - Hit "Set left screen tracker position". Move it to the right lower corner of the screen. Hit "Set right screen tracker position" and click save data.
11. Leave the tracker in the lower right corner stop the playmode and hit Apply Data. Now the tracker should work and you are all ready to do some VP magic. Enjoy

NB.
Sometimes it bugs out and you might have to do the setup twice. 
If the screen looks wrong make sure the "ProjectionPlane" GameObject scale is matchin you VP screen size in meters. If it doesn't set the gameobject manually.
