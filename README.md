# M152ALab1

1. Identify the part of the tb.v where the instructions are sent to the UUT.
   task tskRunInst;
      input [7:0] inst;
      begin
         $display ("%d ... Running instruction %08b", $stime, inst);
         sw = inst;
         #1500000 btnS = 1;
         #3000000 btnS = 0;
      end
   endtask //
2. Which user tasks are called in this process?
    tskRunPUSH
    tskRunMULT
    tskRunADD
    tskRunSEND
