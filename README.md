# download-pdf-without-permission
download-pdf-blocked-permission-drive

```
1. Open Link Drive
2. Load All Page With Scroll Down
3. Paste link hack.js To Console Inspect Element Browser
```

# Message
``` To download a landscape PDF file, basically you have to change line 3 in the code to:
let pdf = new jsPDF('l');

If there's any errors, please use Google Chrome. This is a more specific hint to download a higher quality PDF:
► If I use this line (line 3) in the original code:
                    let pdf = new jsPDF();
then I have a PDF with 297 x 210 (mm) page size.


► To get a higher quality PDF, I have to zoom in the document in Google Drive. I click zoom in button ONE time.
Now I got a bigger image, so I have to increase  297 x 210 (mm)  to  (297*5) x (210*5) (mm) (for example).
So I have to edit line 3 in the code to:
                    let pdf = new jsPDF('p', 'mm', [297*5, 210*5]);
Then I run the code.
In my case, "*5" is good. But it's *4, *6 or even *10, *11 for you, it depends on your file!


► After you find out what page size is good for you document, just do these in order:
1. Go to the document link.
2. Open Console.
3. Click Zoom in.
4. Scroll down slowly.
5. Paste and run the code.
```
