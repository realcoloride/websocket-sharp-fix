# WebsocketSharpFix

This is a fork of sta's [WebsocketSharp](https://github.com/sta/websocket-sharp) that aims at implementing [this PR](https://github.com/sta/websocket-sharp/pull/22).

_I cannot believe this feature is something that has been missing for years._

# Usage of patch

```cs
...
      using (var ws = new WebSocket ("ws://dragonsnest.far/Laputa")) {
            ws.OnMessage += (sender, e) =>
                          Console.WriteLine ("Laputa says: " + e.Data);
            ws.Headers["Cool-Header"] = "Hello world";
            ws.Connect ();
            ws.Send ("BALUS");
            Console.ReadKey (true);
      }
...
```

# Installation 

This should be pretty straightforward. Download/clone the project, build it, and use the `websocket-sharp-fix.dll` as Project reference or import via the Plugins (Unity).

(Use `git clone https://github.com/realcoloride/websocket-sharp-fix` to clone the project)

![image](https://github.com/user-attachments/assets/088f8b3d-f3f3-47ba-87f8-63c0becdd07b)

Make sure to build in Release

![devenv_8Tv6qMxll8](https://github.com/user-attachments/assets/10f0a21f-deb8-4111-91fc-9662aaf28861)
![devenv_2Ig8ihkx9P](https://github.com/user-attachments/assets/bc55bdfd-6f90-4ef3-929e-02fa878cff16)
![devenv_6VQ9ARFLBe](https://github.com/user-attachments/assets/c030ac2e-df8a-4ab0-a7ef-86bc89858d6c)

Good luck with your project!
