CS-204 PROJECT BY:
->CHETAN PRAKASH DUDI:2022CSB1074
->SUMIT TYAGI:2022CSB1131
->MANISH ANWLA:2022CSB1090

Main Function (main()):
 ->Reads input from files named as input1.txt,input2.txt and input3.txt and   extracts branch instructions and outcomes.
->Implements various branch prediction algorithms like always taken,always not taken,1 bit and 2 bit branch predictor.
->Calculates and displays prediction accuracies.
->Writes original branch outcomes, branch target buffer contents, and branch history table to output files.

Helper Functions:
->DecodeInstruction(string bin): Decodes binary instruction to determine if it's a branch instruction or not.
->CalculateOffset(string bin, string inst): Calculates the offset for branch instructions.
->hexStringToBinary(const string &hexString): Converts hexadecimal string to binary string.
->binaryToHexadecimal(const string &binaryString): Converts binary string to hexadecimal string.
->hexToDecimal(const string &hexString): Converts hexadecimal string to decimal.
->intToHex(ll value): Converts decimal value to hexadecimal string.
->displayBTB(): Writes Branch Target Buffer contents to "Branch_Target_Buffer.txt".

Branch Prediction Functions:
->alwaysTakenPredictor(): Implements always taken branch prediction.
->alwaysNotTakenPredictor(): Implements always not taken branch prediction.
->oneBitDynamicPredictor(): Implements one-bit dynamic branch prediction.
->twoBitDynamicPredictor(): Implements two-bit dynamic branch prediction.

Output Files:
->Original_Outcomes.txt: Contains original branch outcomes extracted from input.
->Branch_Target_Buffer.txt: Contains Branch Target Buffer (BTB) contents with current branch address and target address.
->Branch_History_Table.txt: Contains branch history table showing branch addresses and their corresponding prediction outcomes.

Additional Notes:
->Ensure the input file "input3.txt" is present in the same directory as the executable.
->Modify the input file format or file names as needed.
->The code is designed to work specifically with RISC-V machine code instructions.
->The program assumes little-endian architecture for interpreting hexadecimal values.