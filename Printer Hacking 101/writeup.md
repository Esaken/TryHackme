### Printer Hacking 101


*The Internet Printing Protocol (IPP) - is a specialized Internet protocol for communication between client devices and printers. It allows clients to submit one or more print jobs to the printer or print server, and perform tasks such as querying the status of a printer, obtaining the status of print jobs, or canceling individual print jobs.*


What port does IPP run on?
## 631

>we'll be using a Printer exploitation tool

# git clone https://github.com/RUB-NDS/PRET && cd PRET
# 
# python2 -m pip install colorama pysnmP
>most unix machines today run on python3 hence you can use python3

>run the python file 
 # python pret.py

 >this python file executed a program that locates printers
 >an automatic printer discovery in your local network
 >possible to run an Nmap scan however it might take longer and the pret.py scan **only targets ports which printer communication on by default** thus making it faster 


 ### Explooitation
 >run these commands 

```
python pret.py {IP} pjl
python pret.py laserjet.lan ps
python pret.py /dev/usb/lp0 pcl 
```

>Print Server​​ The primary mechanism for Ubuntu printing and print services is the Common UNIX Printing System (CUPS)



### Questions
1. How would a simple printer TCP DoS attack look as a one-line command?
> while true; do nc printer 9100; done

2. Review the cheat sheet provided in the task reading above. What attack are printers often vulnerable to which involves sending more and more information until a pre-allocated buffer size is surpassed?
>buffer overflows

>> USE THE CHEAT SHEET



# use the IP & port provided in the ba example to browse
## http://10.10.243.233:631


3. Connect to the printer per the instructions above. Where's the Fox_Printer located?
> Skidy's basement
4. What is the size of a test sheet?
> 1k


## Task 4

### Done !!!