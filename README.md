# Malicious-XLL-csharp
Malicious excel Plugin (xll) writen in c#

* XLL Downloads a triple-XOR encoded payload. 
* Writes it to memory 
* in memory decryption (only works for x32 office) in this case triple xor. For x64 the decryptor should be modified.

The code included two functions:
* DownloadAndExecute() - Downloads and executes the shellcode
* DownloadAndInject(1231) - Downloads and injects the shellcode to the process with the provided PID


As of 31/07/2022 runs undetected by Defender for Endpoint (used both sliver and metasploit)


A good guide on how to write an excel plugin.
https://bettersolutions.com/csharp/excel-interop/excel-dna-getting-started.htm
