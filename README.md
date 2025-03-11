# block67-r2
The Block67-r2 keyboard was a group-buy keyboard project by ENG Studio from 2022. The project became defunct for some reason. Some people were lucky, like me, and still received the keyboard, though over a year later than advertised, however there was no documentation, and no Via support out of the box.

Below are steps I used to configure the keyboard after struggling for a few hours, hopefully to save someone else a headache. A very simple but annoying issue with this project was that the Function key (Fn) / layer change key is unmapped as it comes out of the box :'(

# Configuration steps
1. Paste the below json into a file, call it ``block67r2.json``.
1. Use a supported browser, navigate to https://www.usevia.app/
1. Go to Settings (https://www.usevia.app/settings)
2. Check "Show Design Tab"
3. Go to Design (https://www.usevia.app/design)
4. Check "Use v2 definitions (deprecated)"
5. Click "Load Draft Definition"
6. Select the ``block67r2.json`` file.
7. Go to Configure (https://www.usevia.app/).
8. Click the key to the left of the left arrow key (between left arrow and right alt). It should start to hover/pulse.
9. Click Layers, then MO(1). This key is now the Fn key. You can change the function of the Fn key by going to Layer 1.


``block67r2.json``, originally posted to the ENG Studio Discord by user r3d_42 (thank you, whoever you are) - I claim no credit whatsoever, but don't want to lose this.

```json
{
    "name": "Block 67 R2",
    "vendorId": "0x7074",
    "productId": "0x1021",
    "lighting": "none",
    "matrix": {"rows": 5, "cols": 15},
    "layouts": {
        "keymap":[
            [{"x":2.5,"c":"#777777"},"0,0",{"c":"#cccccc"},"0,1","0,2","0,3","0,4","0,5","0,6","0,7","0,8","0,9","0,10","0,11","0,12",{"c":"#aaaaaa","w":2},"0,13\n\n\n0,0","0,14",{"x":0.5},"0,13\n\n\n0,1","2,13\n\n\n0,1"],
            [{"x":2.5,"w":1.5},"1,0",{"c":"#cccccc"},"1,1","1,2","1,3","1,4","1,5","1,6","1,7","1,8","1,9","1,10","1,11","1,12",{"w":1.5},"1,13\n\n\n1,0",{"c":"#aaaaaa"},"1,14",{"x":1.25,"c":"#777777","w":1.25,"h":2,"w2":1.5,"h2":1,"x2":-0.25},"1,13\n\n\n1,1"],
            [{"x":2.5,"c":"#aaaaaa","w":1.75},"2,0",{"c":"#cccccc"},"2,1","2,2","2,3","2,4","2,5","2,6","2,7","2,8","2,9","2,10","2,11",{"c":"#777777","w":2.25},"2,12\n\n\n1,0",{"c":"#aaaaaa"},"2,14",{"x":0.25,"c":"#cccccc"},"2,12\n\n\n1,1"],
            [{"c":"#aaaaaa","w":1.25},"3,0\n\n\n2,1",{"c":"#cccccc"},"3,1\n\n\n2,1",{"x":0.25,"c":"#aaaaaa","w":2.25},"3,0\n\n\n2,0",{"c":"#cccccc"},"3,2","3,3","3,4","3,5","3,6","3,7","3,8","3,9","3,10","3,11",{"c":"#aaaaaa","w":1.75},"3,12","3,13","3,14"],
            [{"x":2.5,"w":1.25},"4,0\n\n\n3,0",{"w":1.25},"4,1\n\n\n3,0",{"w":1.25},"4,2\n\n\n3,0",{"c":"#cccccc","w":6.25},"4,6\n\n\n3,0",{"c":"#aaaaaa","w":1.25},"4,10\n\n\n3,0",{"w":1.25},"4,11\n\n\n3,0",{"x":0.5},"4,12","4,13","4,14"],
            [{"y":0.5,"x":2.5,"w":1.5},"4,0\n\n\n3,1","4,1\n\n\n3,1",{"w":1.5},"4,2\n\n\n3,1",{"c":"#cccccc","w":7},"4,6\n\n\n3,1",{"c":"#aaaaaa","w":1.5},"4,11\n\n\n3,1"]
      ],
      "labels":[
            "Split Backspace",
            "ISO Enter",
            "Split Left Shift",
            ["Bottom Row", "6.25U", "7U"]
      ]
    }
}
```
