# RISC-V-MYTH-Workshop
# 3 Digital Logic Design using Tl-Verilog
## A) Combinational Logic:
This TL-Verilog code was implemented on Makerchip, where it defines a simple calculator that takes two random 4-bit numbers and a 2-bit operation selector. It performs addition, subtraction, multiplication, or division based on the selector and assigns the result to $out

         $val1[31:0] = $rand1[3:0];
         $val2[31:0] = $rand2[3:0];
         $op1[1:0] = $rand3[1:0];
         
         
         $sum[31:0] = $val1+$val2;
         $diff[31:0] = $val1-$val2;
         $prod[31:0] = $val1*$val2;
         $quot[31:0] = $val1/$val2;
         
         $out[31:0] = $op[1:0] == 0 ? $sum : $op[1:0] == 1 ? $diff : $op[1:0] == 2 ? $prod : $quot;


