

#### How to import a swift static library. 


#### Put the project in your working space and compile it will generate a .a file. Once Xcode have generated this file 
you have to found the path of the file. 

 Drag and drop the library in the library target section 

1 - Build phase 
2 - look for target library.
3 - drag and drop the file 

#### specify the path of the library  (.a file ): 

1 - Build settings.
2 - look for Search path in the search bar.
3 - look for "Library search path" in this section.
4 - add the search path. 


Note : You can just drag and drop the file in the text window it will automatically write the path for you.

#### Create a Bringing-Header :

In the briging header you will add all your import. 

The header is in the PROJECT_NAME_DIR so this is my import :

\# import "PROJECT_NAME_DIR/mylib-Header.h" // this must be in the Bringing-Header.h file 


#### Final step add the header to the briging Objective-c header : 

1 - Just go in build phase
2 - look for objective-C bringing 
3 - add the file path in the section 
4 - project-name/header.h => here it's project/Bringing-Header.h

