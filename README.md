# MS15-061

****
Exploiting MS15-061 with reverse engineering Win32k.sys by 


****
mail :   Firozimaysam@gmail.com 
twitter : https://twitter.com/R00tkitSMM 


steps :
1. hook PEB callback Function
2. trigger vulnerability ( make proper Window to lead vulnerable function)
3. replace  fack object with NtUserDefSetText in Desktop heap inside PEB callback 
4.  fack object with save exit buffer(0x0c0c0c0c)  and pointer to tagWND 
5.  do it until bServerSideWindowProc is set 
