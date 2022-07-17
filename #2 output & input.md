# JavaScript Output
JavaScript can "display" data in different ways:
* Writing into an HTML element, using *innerHTML.*<br>
    <p>To access an HTML element, JavaScript can use the document.getElementById(id) method.
       The id attribute defines the HTML element. The innerHTML property defines the HTML content:</p>
       
      <!DOCTYPE html>
      <html>
      <body>

      <h1>My First Web Page</h1>
      <p>My First Paragraph</p>

      <p id="demo"></p>

       <script>
       document.getElementById("demo").innerHTML = 5 + 6;
       </script>

      </body>
      </html>

* Writing into the HTML output using *document.write().*<br>
<p>For testing purposes, it is convenient to use document.write():</p>
      <!DOCTYPE html>
      <html>
      <body>

      <h1>My First Web Page</h1>
      <p>My first paragraph.</p>

       <script>
         document.write(5 + 6);
       </script>

      </body>
     </html>
     
* Writing into an alert box, using *window.alert().*<br>
<p>We can use an alert box to display data:<p>
    <!DOCTYPE html>
    <html>
     <body>

     <h1>My First Web Page</h1>
     <p>My first paragraph.</p>

     <script>
     alert(5 + 5);
    </script>

    </body>
  </html>
  
* Writing into the browser console, using *console.log().*<br>
  <p>For debugging purposes, you can call the "console.log(..)" method in the browser to display data.
  However, using "console.log(..)" is generally going to make learning about coding and running your program in 
  the console easier than rest of the oputput methods. so for this Tutorial, we'll use "console.log(..)" for output.</p>
      a = 21;
      b = a * 2;
      console.log( b );
      
      //output 42
      //Go and try it in your browser console.
  
# Javascript Input
 <p>While we are discussing output, you may also wonder about *input*(i.e., receving information from the user).
 The most common way that happens is for HTML page to show form element (like text box) to a user that he/she can type into, and 
 then use JS to read those values into your program;s variables.

 But there's an easier way to get input for simple learning and demonstration purpose such as what you'll be doing throughout this guide. 
 Use the "prompt(..)" function.</P>

      age = prompt( "please tell me your age:" );
      console.log( age );
      
 in this case "please tell me your age:" --is printed into a popup ans once you submit it after entering the value it should reflect the same in         console.log(..).
   
# conclusion 
  So we learned about how we get OUTPUT and INPUT in Javascript.<br>
  Thankyou.
