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

# Installation (soon)
