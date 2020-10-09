# Rasat Android

The package adds to [Rasat Java](https://github.com/s4ysolutions/rasat-java) the ability to
broadcast the event through predefined android handler.

The code below ensure all handlers added to the channel observers are called in the main thread

```
import solutions.s4y.rasat.android;

Channel channel = new Channel(new Handler(Looper.getMainLooper())
```