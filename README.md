# youTile
A tiny little program for nesting rectangular pieces on rectangular sheets (primarily for cutting).

## How it works
The program consists of a single .html file with some javascript to be opened by your preferred web browser on a desktop platform you use. It is simple, it is stupid even more and it was made so intentionally ([KISS principle](https://en.wikipedia.org/wiki/KISS_principle)!). Built-in capabilities of modern browsers allow to keep the code compact and without any dependencies. The program file [youTile.html](./youTile.html) is the code, so you can tweak it for your needs by editing the file contents directly.

youTile provides basic interface to create a list of rectangular parts with their respective dimensions and quantities (aka Bill of Materials). You can then nest them on sheets of specified size and plan how many sheets of each kind you will need to realize the inventory. There are no suggestions on the optimum nesting, it justs plots everything in scale, saving time on drawing by hand and tackling with general purpose design software, but not replacing your imagination and creativity (hence the name: "You Tile"). Additionally it takes care about the width of the cutting tool to provide gaps between the parts.

## Reference
On the left hand side, there is a green pad for some general information such as customer's name and material type. These fields may be left empty or edited afterwards. However, you would like to specify the cutting kerf width before you start nesting your parts, as it will affect snapping them in place with proper gaps.

### Parts
Next, you can fill information about the parts. These fields are interactive: other numbers and graphical representation will be updated accordingly once the field content is changed. The "Left" column denotes how many parts are still not in the layout on the right hand side. The red cross on each line deletes the respective part from the list and from the layouts. Press "more..." button to add a new part.

### Sheets
Same thing works for the sheets, except that every line has its sheet drawn right beneath. Interactivity holds here as well.

### Nesting layouts
Finally, nesting! Click anywhere in the sheet area and choose the part you want to place there from a drop down list. Left mouse click on the part flips its sides, right mouse click removes the part from the sheet. Drag it anywhere you want to place, note the sticky action when it meets sheet borders or other parts. You can even drag it to another sheet!

### Remarks
Asterisks * on the left and after every sheet provide place for free form comments and remark (such as "Do it NOW!").

### Output
Once you are satisfied with the layout, print it right away from the browser (Ctrl+P should work as well as File->Print or right mouse click -> Print). Options like "Print to file" or "Save as PDF" in the print dialogue allow to save the layout in a printable way as PDF.

Printing drops some unnecessary information, such as kerf width and "Left" column. Particularly important text is enlarged for easier reading. Some browsers (like Opera) offer "Save as PDF" option in context menu (on right mouse click), this will produce a one (probably long) page document "as is".

### Miscellaneous
youTile updates the "Left" column in accordance with the visual description and "Qty." values. However, please note that every part belongs to some sheet even if it lays outside. Vertical position of the top side of the part determines which sheet it belongs to. Anyway, an adequate location of parts is treated adequately.

## Possible uses and other tools
youTile is a small utility, straightforward to learn and use. Although it was developed to simplify day to day routine of cutting sheet material for customer needs, it may find other uses in planning of tiling, parquet flooring or wallpapering.

For truly smart nesting software, take a look at [MaxCut](https://www.maxcutsoftware.com), [iNEST](http://www.i-nesting.com/), [MyNesting](https://www.mynesting.com), [Magi-Cut](https://www.magi-cut.co.uk/cloud/), [SVGnest](https://svgnest.com), [GoNest 2D](http://www.gonest2d.com),  and others.
