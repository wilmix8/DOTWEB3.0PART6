# JWEB6.0
==========


JWEB6.0  is also   called  as  JSHIELD which  is  invented   by  wilmix  jemin  j  at  year  2017

is  focused  for  high  security  with  encoding  and  decoding  the  text  with  encryption.


What  is  the  Work flow  of  JWEB6.0?
======================================

When  remoteserver   compiles  .Jdollar

it  generates  a  .class  file  and  .bs file  that  we already know.

When  .bs  is  invoked  in our browser  it  converts  to  .S  file and  deletes  .class file   ie)

.S  is  called  as  Security file for  future  use.

When  you  invoked  in  your  browser  the  security  file  .S  contents  is  displayed.



  

SYNTAX-1
==========



<JDollar>
@JRemote



 

<%




public class index {


  public void  JDOLLAR-Main( )
{


<! JDollar  security logic !>

 
}

}



%>


</JDollar>





SYNTAX-2
========

filename.j$
===========

<JDollar>

<USE> <WEB>.util;


<PACK> Program5
{
  
    <CLASS> Prog
   {

  
      public void Main()
      {

<!  JDollar  logic  !> 

		
}


}

}


note: here  you  can  use  .dll  file 

in  properties  file  and  use  the  libraries  in the  main program.


Example1-1:
===========

<JDollar>
@JRemote



 

<%




public class index {


  public void  JDOLLAR-Main( )
{


HTML.displayhtml("Register.html");


 
}

}



%>


</JDollar>





Jquerytest.j$
=============


<JDollar>

<USE> <WEB>.util;


<PACK> Program5
{
  
    <CLASS> Prog
   {

  
      public void Main()
      {

ArrayList arm1= new ArrayList();

arm1.add("name");
arm1.add("uname");arm1.add("password");
arm1.add("state");
arm1.add("coun<TRY>");
arm1.add("spwd");
arm1.add("stext");
arm1.add("familydet");
arm1.add("Indent");
arm1.add("CIndent");

arm1.add("NOT");

<PRINTLN>("<HTML>");

<PRINTLN>("<BODY bgcolor=pink>");

<PRINTLN>("<form>");
 
  
// security  file  parameters will  store  it  in  filename.sl.dsn format

ArrayList  armg= Request.Query(arm1,"index.sl.dsn",10,1);
 <PRINTLN>("<table style='width:100%' bgcolor=gold>");

<PRINTLN>("<tr>");

<PRINTLN>("  <th>Name</th>");
  
<PRINTLN>("  <th>Username</th>"); 
  
<PRINTLN>("  <th>Password</th>");
  
<PRINTLN>("  <th>State</th>");
  
<PRINTLN>("  <th>Country</th>");
  
<PRINTLN>("  <th>Confirm Password</th>");

<PRINTLN>("  <th>Secret Password</th>");

<PRINTLN>("  <th> FamilyDetails </th>");
<PRINTLN>("  <th>Percentage of Marks Scored</th>");
<PRINTLN>("  <th>Subject</th>");
   
<PRINTLN>(" </tr>");
   
<PRINTLN>(" <tr>");



for (int i=armg.size()-10;i<armg.size();i++)
{


   <PRINTLN>("<td>"+armg.get(i)+"</td>");
   
 }

  
<PRINTLN>(" </tr>");
 
  
<PRINTLN>("</table>");


<PRINTLN>("</form>");

<PRINTLN>("</html>");
      
 

		
}


}

}



Note:  JWEB6.0   is  focused  on  security   projects  like  school  marks  mgt,etc.
====
JWEB6.0   is  used  with  JDollarpart1  and JDollarpart2.









