
# File Compressor and Decompressor
Made a GUI to compress a txt file into a gzip file and decode the encoded text file (compressed into gzip
file). Was able to compress a file of size 2668 kb to 5kb.

# GUI 
https://user-images.githubusercontent.com/74968170/196412431-26733d97-5a90-449f-8e1e-2f069eab5fce.mp4

# Dtails of Projects 
basically there is a two part of project where in one part we are basically compressing a file and another part again decompessing again.
# Compress java :

              public class Compress {
                 public static void method(File file) throws IOException{
                  String fileDirectory =file.getParent();
                  System.out.println(fileDirectory);
                  FileInputStream fis = new FileInputStream(file);
                  FileOutputStream fos = new FileOutputStream(fileDirectory + "/Comptreddedfile.gz");
                  GZIPOutputStream gzipOS = new GZIPOutputStream(fos);
                  byte []buffer = new byte[1024];

                  int len;
                  while((len=fis.read(buffer)) !=-1){
                      gzipOS.write(buffer,0,len);
                  }
              gzipOS.close();
              fos.close();
              fis.close();
                 } 
                 public static void main(String [] args)throws IOException{
                     File path=new File("C:\\Users\\arvin\\OneDrive\\Desktop\\resume\\text.txt");
                     method(path);
                 }
              }

here we are using FileInputStream() to take a input stream and FileOutputStream for saving the files with sama parents directry . GZIPOutputStream gzipOS = new GZIPOutputStream(fos) this is the main method which will giving the compress file in the form of objecs.we are also making buffer array to compress line by line each word according to our requirments ,we are taking a input txt file in main method and passed the method to compress.
# Decompress .java 

# Java Swing and awt
AWT and Swing are used to develop window-based applications in Java. Awt is an abstract window toolkit that provides various component classes like Label, Button, TextField, etc., to show window components on the screen. All these classes are part of the Java.awt package.

On the other hand, Swing is the part of JFC (Java Foundation Classes) built on the top of AWT and written entirely in Java
. The javax.swing API provides all the component classes like JButton, JTextField, JCheckbox, JMenu, etc.

The components of Swing are platform-independent, i.e., swing doesn't depend on the operating system to show the components. Also, the Swing's components are lightweight.


# Conclusion
By now I’m sure you understand exactly how our traversal algorithm could generate the path shown in above video. Which is just one of a couple of available paths. We learned about some graph theory, depth-first search, the call stack and how all of it applies to finding a path through a maze. I hope y’all enjoyed reading this article as much as I enjoyed writing it!

## Authors

- [@arvind171219](https://www.github.com/octokatherine)


## Documentation

[Documentation](https://linktodocumentation)

