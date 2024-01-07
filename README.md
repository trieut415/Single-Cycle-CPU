1. Add instruction SLT. Hint: you only need to modify the ALU and ALU control logic.
In our addition of SLT, we just added an additional function in ALU Control under our R-type
commands, and gave it a new function number to map to. Then, after we modified that, we
handled it in the ALU, where we created a new function using the ternary operator in the
following format R[rd] = R[rs] < R[rt] ? 1 : 0


2. Add instruction ADDI. You do not need to general support for I-Format ALU instructions.
Hint: you can do this without adding any new hardware, i.e., just by modifying the control.
In our addition of addi, we just added an additional function in ALU Control under our R-type
commands, and gave it a new function number to map to. Then, after we modified that, we
handled it in the ALU, where we simply added the two input values together and assigned that
to the output.


4. Add instruction J. Use the implementation in the text. [Start in pre-lab]
In our implementation of jump, we essentially just followed in the diagram in the discussion, we
added a new multiplexer after the ALUresult.


5. Add instruction BNE.
In our implementation of BNE, we extended the bit size of ALU op and created a specific
function for it in our ALU_control.


6. Add instruction LUI
In our implementation of LUI, we extended the bit size of ALU op, and added handling in control.
