# OG-star-tracker-

This fork is to be able to use my NEX-5T camera from the tracker. They don't have a way to use the snap port conventionally, so
I'm stuck have to hack together a solution. This is unproven, I still haven't received my star tracker so I can't know if it will work until
it arrives and I assemble it.

I ended using a infrared controller [like this one](https://www.amazon.com/JJC-RMT-DSLR1-Wireless-Remote-Control/dp/B06Y69KRYZ) that can send a shutter release 
command to the camera. I modified it, adding two wires to both pads that make up the key so that I can electrically "press" it.

The controller works in a certain way:
- It won't trigger the camera until you let go of the button and press it again once it has finished saving the picture.
- In any mode that isn't BULB, a single press makes it take a full picture.
- In BULB mode, when you send a signal it will start the capture and it will not stop until it receives another one.

I plan on supporting the camera in BULB mode, sending a brief pulse to the controller to start the capture and another one to stop. Also, it is quite slow to save the pictures to
the SD card, so I'm going to make the delay modifiable by the user.

## Plans
- Add a new rutine to the FW to support the IR controller.
- Add a check-box to select whether it's a normal snap port or a IR controller.
- Add a new box to write what should be the delay.

## Original README below

Is a fully 3d printed upgradable star tracker that you can make for 60$, I have been working on it for the past two years. It can handle
up to 300mm and 2.5kg. It's also upgradable which means that you can add a another axis which would allow you to use go-to.Don't hesitate to ask me. 
- [List of parts](https://docs.google.com/spreadsheets/d/1kcgIab0JqNLg5WMselIyCQLZJsu3P-vXLvSJgl1yHa8)
- [Assembly video](https://www.youtube.com/watch?v=97YKJrmOWHY)

I plan on selling it in future for around 150$. There is a [discord](https://discord.gg/dyFKm79gKJ) for those who are
interested or would want to ask me a few questions. New STLs are
on [printables](https://www.printables.com/model/348574-og-star-tracker).

## License

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-nc-sa/4.0/)

[![CC-BY-NC-SA 4.0](https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png)](http://creativecommons.org/licenses/by-nc-sa/4.0/)
