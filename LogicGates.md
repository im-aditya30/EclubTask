<style
  type="text/css">

table {
  /* */
  /* border: 1px solid black; */
}
.box {
  width: 158px;
  text-align:center;
  margin:0 auto;
}
th{
  /* background-color:#000000; */
  color:#FFFFFF; 
  
}
</style>




# Logic Gates
   <h3>What are Logic Gates?</h3>
   Logic gates are the basic building blocks of any digital circuit. They are electronic circuits which have one or more inputs and only one output which relates to the input signals based on a certain logic.

  ##### These are the basic logic gates:<br>
  <h4>  

  * AND Gate
  </h4> <br>
<p >
  <a href ="https://www.electronicshub.org/digital-logic-and-gate/"><img src= "/images/and.jpg" alt ="AND Gate Symbol"></a><br> AND Gate Symbol
 </p><br>
 <div class="box">
 <table  >
    <tr>
      <th colspan ="2"> Input</th>
      <th> Output</th>
    </tr>
    <tr>
      <th>X</th>
      <th>Y</th>
      <th>Z</th>
    </tr>
    <tr>
      <td>0</td>
      <td>0</td>
      <td align="center">0</td>
    </tr>
    <tr>
      <td>0</td>
      <td>1</td>
      <td align="center">0</td>
    </tr>
    <tr>
      <td>1</td>
      <td>0</td>
      <td align="center">0</td>
    </tr>
    <tr>
      <td>1</td>
      <td>1</td>
      <td align="center">1</td>
    </tr>
  </table>
 </div>
  <p align = "left">AND Gate Truth Table</p><br>

  <h4>  

  * OR Gate
  </h4> <br>
  <p align = "left">
  <a href ="https://www.electronicshub.org/digital-logic-or-gate/"><img src= "/images/or.jpg" alt ="OR Gate Symbol"></a><br> OR Gate Symbol
 </p><br>
 <table align = "left" class="box">
    <tr>
      <th colspan ="2"> Input</th>
      <th> Output</th>
    </tr>
    <tr>
      <th>X</th>
      <th>Y</th>
      <th>Z</th>
    </tr>
    <tr>
      <td>0</td>
      <td>0</td>
      <td align="center">0</td>
    </tr>
    <tr>
      <td>0</td>
      <td>1</td>
      <td align="center">1</td>
    </tr>
    <tr>
      <td>1</td>
      <td>0</td>
      <td align="center">1</td>
    </tr>
    <tr>
      <td>1</td>
      <td>1</td>
      <td align="center">1</td>
    </tr>
  </table>
  <p align = "left">OR Gate Truth Table</p><br>

  <h4>  

  * NOT Gate
  </h4> <br>
   <p align = "left">
  <a href ="https://www.electronicshub.org/digital-logic-not-gate/"><img src= "/images/not.jpg" alt ="NOT Gate Symbol"></a><br> NOT Gate Symbol
 </p><br>

 <p align = "left">
  <table align = "left" class="box">
    <tr>
      <th colspan ="1"> Input</th>
      <th> Output</th>
    </tr>
    <tr>
      <th>X</th>
      <!-- <th>Y</th> -->
      <th>Z</th>
    </tr>
    <tr>
      <td align = "left">0</td>
      <!-- <td>0</td> -->
      <td align="center">1</td>
    </tr>
    <tr>
      <td align = "left">1</td>
      <!-- <td>1</td> -->
      <td align="center">0</td>
    </tr>
  </table>
  </p>

  <p align = "left">NOT Gate Truth Table</p><br>

  <h4>  

  * NOR Gate
  </h4> 

  <p align = "left">
    <img src= "/images/nor.jpg" alt ="NOR Gate Symbol"> <br> NOR Gate Symbol
 </p><br>

 <table class = "box">
    <tr>
      <th colspan ="2"> Input</th>
      <th> Output</th>
    </tr>
    <tr>
      <th>X</th>
      <th>Y</th>
      <th>Z</th>
    </tr>
    <tr>
      <td>0</td>
      <td>0</td>
      <td align="center">1</td>
    </tr>
    <tr>
      <td>0</td>
      <td>1</td>
      <td align="center">0</td>
    </tr>
    <tr>
      <td>1</td>
      <td>0</td>
      <td align="center">0</td>
    </tr>
    <tr>
      <td>1</td>
      <td>1</td>
      <td align="center">0</td>
    </tr>
  </table>
  <p align = "left">NOR Gate Truth Table</p><br>

  <h4>  

  * NAND Gate
  </h4> <br>
  <p align = "left">
  <a href ="https://www.electronicshub.org/universal-gates-nand-gate/"><img src= "/images/nand.jpg" alt ="NAND Gate Symbol"></a><br> NAND Gate Symbol
 </p><br>
 <table align = "left" class="box">
    <tr>
      <th colspan ="2"> Input</th>
      <th> Output</th>
    </tr>
    <tr>
      <th>X</th>
      <th>Y</th>
      <th>Z</th>
    </tr>
    <tr>
      <td>0</td>
      <td>0</td>
      <td align="center">1</td>
    </tr>
    <tr>
      <td>0</td>
      <td>1</td>
      <td align="center">1</td>
    </tr>
    <tr>
      <td>1</td>
      <td>0</td>
      <td align="center">1</td>
    </tr>
    <tr>
      <td>1</td>
      <td>1</td>
      <td align="center">0</td>
    </tr>
  </table>
  <p align = "left">NAND Gate Truth Table</p><br>
<h4>  

  * XOR Gate
  </h4> <br>
  <p align = "left" >
  <a href ="https://www.electronicshub.org/universal-gates-nor-gate/"><img src= "/images/xor.jpg" alt ="XOR Gate Symbol"></a><br> XOR Gate Symbol
 </p><br>
 <table align = "left" class="box">
    <tr>
      <th colspan ="2"> Input</th>
      <th> Output</th>
    </tr>
    <tr>
      <th>X</th>
      <th>Y</th>
      <th>Z</th>
    </tr>
    <tr>
      <td>0</td>
      <td>0</td>
      <td align="center">0</td>
    </tr>
    <tr>
      <td>0</td>
      <td>1</td>
      <td align="center">1</td>
    </tr>
    <tr>
      <td>1</td>
      <td>0</td>
      <td align="center">1</td>
    </tr>
    <tr>
      <td>1</td>
      <td>1</td>
      <td align="center">0</td>
    </tr>
  </table>
  <p align = "left">XOR Gate Truth Table</p><br>
  
  <h4>  

  * XOR Gate
  </h4> <br>
  <p align = "left">
  <a href ="https://www.electronicshub.org/universal-gates-nor-gate/"><img src= "/images/xnor.jpg" alt ="XNOR Gate Symbol"></a><br> XNOR Gate Symbol
 </p><br>
 <table align = "left" class="box">
    <tr>
      <th colspan ="2"> Input</th>
      <th> Output</th>
    </tr>
    <tr>
      <th>X</th>
      <th>Y</th>
      <th>Z</th>
    </tr>
    <tr>
      <td>0</td>
      <td>0</td>
      <td align="center">1</td>
    </tr>
    <tr>
      <td>0</td>
      <td>1</td>
      <td align="center">0</td>
    </tr>
    <tr>
      <td>1</td>
      <td>0</td>
      <td align="center">0</td>
    </tr>
    <tr>
      <td>1</td>
      <td>1</td>
      <td align="center">1</td>
    </tr>
  </table>
  <p align = "left">XNOR Gate Truth Table</p><br>

  The NAND (NOT-AND) and NOR (NOT-OR) gates are considered universal gates and can be used to make any other logic gate.<br> For example : NAND gate can be use to make following gates:<br>
 <p align = "left">
  <img src ="/images/nandgateUses.webp" alt ="NAND Gate Uses">
 </p>
 <hr>
 
