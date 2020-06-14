## Past Projects

### [Report Failed Backups](https://github.com/AkiliKhasi/CompareList)

Our backup software would send daily reports as a PDF for every customer and their corresponding DR site. In order for a manager to see if a report had not been run for a specific customer they would have to sort through a list of over 150 PDF files to see if it was missing. In order to make this process more efficient I wrote this script to compare all of the PDF files generated that day against a control list and then list any missing reports in a text file.   

### [Set Default Applications](https://github.com/AkiliKhasi/SetDefaultApplications)

After a Windows update reset the default applications for all of our client's computers we needed a way to set the defaults on every PC. The first step was to create an XML file with the default applications and then use a DISM command on every PC to import the settings from the XML file. This did work but running the DISM command on hundreds of PCs manually would have been very time consuming and taken weeks to complete. I wrote this script to automate that process by using a CSV file with all of the PC names and then using powershell to run the DISM command remotely against every PC in the list.

### [Automated PC Setup](https://github.com/AkiliKhasi/BenchScript)

When we received new PCs for any client we would have to remove any software from the manufacturer and set some default settings within Windows. We would then have to install the latest versions of Adobe and Jave before shipping the PC to the client. I wanted to automate this proccess so I wrote this script that removes any bloatware from HP or Dell and any trial editions of Microsoft Office. The script also changes some settings within Windows for the Windows Firewall, Power Settings, and UAC then installs the latest version of Adobe Reader and Java.
