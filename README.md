[![Work in Repl.it](https://classroom.github.com/assets/work-in-replit-14baed9a392b3a25080506f3b7b6d57f295ec2978f6f33ec97e36a161684cbe9.svg)](https://classroom.github.com/online_ide?assignment_repo_id=4709263&assignment_repo_type=AssignmentRepo)
# Chapter-2-Lab-8b

Lab Goal :  This lab was designed to teach you more about a linked list and using a linked list in a class as an instance variable / data field.

Lab Description :   Use   ListNode   to write some basic LinkedList methods.  

PART 1 – Open the   ListFunHouseTwo.java   file and complete the methods in this class.   
PART 2 – Use the   Main  to test your   ListFunHouseTwo  class.

Files Needed ::

ListNode.java
Linkable.java
ListFunHouseTwo.java
Main.java


ListNode – stores a value and a reference to the next node
public class ListNode implements Linkable
 {
   private Comparable listNodeValue;
   private ListNode nextListNode;

   public ListNode(){
      listNodeValue = null;
      nextListNode = null;
   }

   public ListNode(Comparable value, ListNode next){
       listNodeValue=value;
      nextListNode=next;
   }

   public Comparable getValue(){
      return listNodeValue;
   }

   public ListNode getNext(){
      return nextListNode;
   }

   public void setValue(Comparable value){
      listNodeValue = value;
   }
 
   public void setNext(Linkable next){
      nextListNode = (ListNode)next;
   }
}

Sample Data : 
See Main.

Sample Output :
Original list values
over up -a-2-1 2.1 34 at on go

num nodes = 8

List values after calling nodeCount

over up -a-2-1 2.1 34 at on go

List values after calling doubleLast

over up -a-2-1 2.1 34 at on go go

List values after calling doubleFirst

over over up -a-2-1 2.1 34 at on go go

List values after calling removeXthNode(2)

over up 2.1 at go

EXTENSION :  Modify ListNode by adding in a     ListNode prevListNode   instance variable / data field.   Rewrite the program as a double/circular linked list.


