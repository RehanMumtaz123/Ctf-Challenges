#### SOLUTION 
##### Challenge 2 Easy (XORcery) 

1. Open the pcap file in the wireshark.
2. Right click the http packet > follow > http stream
3. There is http call endpoint `/update` where address value is in hex encoded, copy that and remove `+` between the values and change it to ascii
4. Upon decoding there is a python code (decryptor).
5. Next is to find encrypted flag.
6. There is another endpoint in the stream `/guest` where the body param contains base64 enc & encrypted value 
7. Just pass it as the parameter in the decryptor code and that will give out the flag 

✌
