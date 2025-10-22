markdown

<img width="1536" height="1024" alt="bash" src="https://github.com/user-attachments/assets/ac0ebd07-ffd5-4f71-bf3e-133e4e4e50a3" />


---

## Menu display list
- Show disk usage
- Show ip address
-  Show running process
-  Exit the menu.sh

---

## 1. Create the script file
Open your terminal and run this command to create new file menu.sh
```bash
$ nano menu.sh
```

---

## 2. Add this script content
```bash
#/bin/bash
# A simple menu script

while true; do
    echo "-----------"
    echo "    SYSTSEM MENU"
    echo "1. show disk usage"
    echo "2. show ip address"
    echo "3. show running process"
    echo "4. Exit"
    echo "-----------"
    read -p "Enter your choice [1-4]:" choice

    case $choice in
        1)
           echo "Disk usage"
           df -h
           ;;
        2)
           echo "Ip address"
           hostname -I
           ;;
        3)
           echo "Running process"
           ps aux
          ;;
        4)
           echo "Exiting... Goodbye"
           break
        *)
           echo "Invalid option, Please choose between 1-4."
           ;;

    esac


    echo ""
    read -p "Press Enter to continue..."
    clear
done
```
After that Press Ctrl + O to save, Enter to confirm, and Ctrl + X to exit the Nano editor.

---
 ## Make the file excutable
 ```bash
$ chmod +x menu.sh
```

---

When you run the script, you'll something like this

-----------
    SYSTEM MENU
1. Show disk usage
2. Show IP address
3. Show running processes
4. Exit
-----------
Enter your choice [1-4]:

Images from the output


<img width="644" height="232" alt="Disk_usage" src="https://github.com/user-attachments/assets/fb004c54-61d2-4029-83ba-c762d3f50b47" />


---


<img width="1097" height="72" alt="Ip_address" src="https://github.com/user-attachments/assets/87633d62-f413-47a0-8078-076184bd1969" />


---


<img width="483" height="288" alt="menu sh" src="https://github.com/user-attachments/assets/997635bf-ee8f-4582-8a80-5c47ed4cf733" />


---


<img width="1091" height="443" alt="Running_process" src="https://github.com/user-attachments/assets/761dc19f-0418-4e45-9172-9ae652a3819f" />




















