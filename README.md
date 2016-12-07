# Assignment8.3
package com.session8;

import java.io.File;
import java.io.FileInputStream;
import java.io.FileNotFoundException;
import java.io.FileOutputStream;
import java.io.IOException;

public class Filecopy {

	public static void main(String[] args) throws IOException {
		// TODO Auto-generated method stub
	//	Desktop
     FileInputStream fin = new FileInputStream("C:\\Users\\Unni\\Desktop\\Emp.txt");
	int data = fin.read();
	 FileOutputStream fout = new FileOutputStream("C:\\Users\\Unni\\Desktop\\xyz.txt");
	 while (data!=-1){
		 fout.write(data);
		 data = fin.read(); 
	
	 }
	 fin.close();
	 fout.close();
}
	
}
