# Lab2C-LoadImage
**(Optional)** Learn how to load an image file. 

1. Open a new Processing file. Inside of your lab 2 folder, save your file within the lab 2 folder as as `Lab2C-*YOUR FIRST NAME*-*YOUR LAST NAME*`.
2. Add your opening comments.
```processing
/*  Lab 2C (Optional) - NMD 211
    FirstName LastName
    September 18, 2020
    
    
    Load an image. PNG files with transparent background preferred. 
    
    If the image is not yours, link to the source in the readme. 
    
    (if you want to do something extra: Make the image part of a class object, 
    and do something interesting with the image.)
*/
```
3. Create a global image object. 
```processing
/*  Lab 2C (Optional) - NMD 211
    FirstName LastName
    September 18, 2020
    
    
    Load an image. PNG files with transparent background preferred. 
    
    If the image is not yours, link to the source in the readme. 
    
    (if you want to do something extra: Make the image part of a class object, 
    and do something interesting with the image.)
*/
PImage img;
```
4. Add your normal set up information. We will be loading images, so add imageMode(CENTER). This means that any images will be anchored onto your drawing space from their centerpoint, not a corner. 
```processing
PImage img;

void setup(){
   size( 500 , 500);              // drawing space size
   
   imageMode(CENTER);
}
```
5. Load your image. Mine is called "sample.png" and saved in the same folder as my processing `.pde` file.  
```processing
PImage img;

void setup(){
   size( 500 , 500);              // drawing space size
   
   imageMode(CENTER);
   
   img = loadImage("sample.png");
}
```
6. Resize your image as necessary.
```processing
PImage img;

void setup(){
   size( 500 , 500);              // drawing space size
   
   imageMode(CENTER);
   
   img = loadImage("sample.png");
   img.resize(width/2, 0);       // resizes image to a width of the page size 
                                 // but keeps proportions of height  
}
```
7. Draw your image. 
```processing
PImage img;

void setup(){
   size( 500 , 500);              // drawing space size
   
   imageMode(CENTER);
   
   img = loadImage("sample.png");
   img.resize(width/2, 0);       // resizes image to a width of the page size 
                                 // but keeps proportions of height  
}

void draw(){
  background( 255, 245, 175);
  image( img, width/2, height/2); // loads image img at x = page width/2, y = page height/2 
}
```
## Submit your Lab
[FirstName LastName - 2C](http://example.com)
