# Reverse-Engineering-Practice-Task-01

public class BBAStudent extends Student{

  private String name = " ";  
  private String department = "BBA";
  
  public BBAStudent(){
   this.name="Default BBA Student";
  }
  
    public  BBAStudent(String a){
   
      this.name=a;
  }
  
  
  
  
  
  public String toString(){
    return "Name : " + name + " Department: " + department;
  }
  
  
  
  
}

\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\

public class Student{
  private String name = "Just a Student";  
  private String department = "nothing";
  public void setDepartment(String dpt){
    this.department = dpt;
  }
  protected String getName(){
    return name;
  }
  protected void setName(String name){
    this.name = name;
  }
  public String toString(){
    return "Name : " + name + " Department: " + department;
  }
}


\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\

import java.util.*;

public class TestStudent{
  public static void printName(Student s){
    System.out.println(s.toString());
  }
  public static void main(String [] args){
    printName(new BBAStudent());
    printName(new BBAStudent("Humty Dumty"));
    printName(new BBAStudent("Little Bo Peep"));    
  }
}



