# nicokeeb

He wants to ease himself into weird keyboards. 
He said he like the ortholinear rather than column stagger for now. 
So maybe make a 14x5 ortho with an inverted t cursor section.

    points:
      mirror:
        ref: ortho_inner_home
        distance: 1U
      zones:
        ortho:
          columns:
            farfarpinky:
            farpinky:
            pinky:
            ring:
            middle:
            index:
            inner:
          rows:
            mods:
            bottom:
            home:
            top:
            nums:


    [{a:7},"`","1","2","3","4","5","6","7","8","9","0","-","+","DEL",{x:0.25},"","",""],
    ["Tab","Q","W","E","R","T","Y","U","I","O","P","[","]","\\",{x:0.25},"","",""],
    ["Ctrl","A","S","D","F","G","H","J","K","L",";","'","","",{x:0.25},"","",""],
    ["Shift","Z","X","C","V","B","N","M",",",".","/","Shift","","",{x:1.25},"&uarr;"],
    ["","Ctrl","Alt","Super","&dArr;",{w:2},"","","","","","","","",{x:0.25},"&larr;","&darr;","&rarr;"]

Now with full 5x5 parts

    [{a:7},"`","1","2","3","4","5","6","7","8","9","0","-","+","DEL","",{x:1},"","",""],
    ["Tab","Q","W","E","R","T","Y","U","I","O","P","[","]","\\","",{x:1},"","",""],
    ["Caps","A","S","D","F","G","H","J","K","L",";","'","","","",{x:1},"","",""],
    ["Shift","Z","X","C","V","B","N","M",",",".","/","Shift","","","",{x:2},"&uarr;"],
    ["Ctrl","Win","Alt","Super","",{w:2},"","","","","","","","","",{x:1},"&larr;","&darr;","&rarr;"]



Using three 5x5 parts we will get a 15x5 ortho which will use 15+5=20 pins unoptimized.

If we used four 5x5 parts we will need 20+5=25 pins. The Pico has 26 gpio so that should work.

If we could optimize it to be a 2x2 grid of the 5x5 parts then it would only need 10+10=20 pins.
