# llvm-fla-cracker
## Introduction
The goal of the llvm-fla-cracker is to retrieve the normal execution program flow from its disorderd form which is made by the llvm obfuscator with compling option "-fla" (https://github.com/obfuscator-llvm/obfuscator ).  There are also other two sorts of obfuscation in the llvm obfuscator with compling option "-sub" and "-bcf". But temporarily these two are not within my interest. 

## How to use
  <1> Use IDA to get the pseudocode. Save the pseudocode in a file (note: please use ctrl + A to copy the pseudocode, and don't modify  it. `All the numbers appeared in the comparasion should be in decimal. `. Because temporarily the python script relies on the code text format extremely.). The pseudocode may look like the 5 given testcodes. </br>
  <2> Let's roll by using "python llvm_fla_cracker_simple.py inputfile outputfile", where inputfile and outputfile can be freely defined. For example, use "python llvm_fla_cracker_simple.py testcode3.txt 3.txt" you will get a "neat" code of testcode3.txt in file "3.txt".


