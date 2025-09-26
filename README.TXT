Project: music-organizer-v3. A project to collect audio files.
Authors: David J. Barnes and Michael Kölling

This project is part of the material for the book

   Objects First with Java - A Practical Introduction using BlueJ
   Seventh edition
   David J. Barnes and Michael Kölling

It is discussed in chapter 4.

To start:

Create a MusicOrganizer object on the object bench.
Use its methods to add, remove, and play files. The listAllFiles
method prints a list of the collection.

Challenge Exercise 24:

/**
 * Show a list of all the files in the collection
 * with their index numbers.
 */
public void listWithIndex()
{
    int position = 0;  
    for(String filename : files) {
        System.out.println(position + ": " + filename);
        position++
    }
}

25:

public void listMatching(String searchString)
   {
       for(String filename : files) {
           if(filename.contains(searchString)){
               System.out.println(filename);
           }
       }
   }
   
26: public void listMatching(String searchString)
   {
       boolean found = false;
       
       for(String filename : files) {
           if(filename.contains(searchString)){
               System.out.println(filename);
               found = true;
           }
       }
       
       if(found == false) {
           System.out.println("No files containing: " + searchString + " found");
       }
   }
    

    
    
    
