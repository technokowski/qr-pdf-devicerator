# qr-pdf-devicerator
Generates pdfs from a supplied csv which include a QR code with the data of each row

During the pandemic we issued out thousands of chromebooks, and now we have to turn them all in. It's a giant undertaking,
so I designed this to speed up the process and make the data accurate on the day of returns. 

What is this thing? It takes a csv with four columns; Name, email, asset tag, department. 

It generates a pdf that includes a qr code with all of the above mentioned row data, as well as some info on why it's important to
turn in the correct one. This way users can turn in their device, scan the printed copy (which gives them credit for turning in
a device), and records missing items for the purpose of reporting and audits.

To run the program, just execute from the directory of main.py, and supply a csv from cli, for example:

python3 /User/qr-pdf-devicenator/main.py user_data.csv


The program takes the csv file as an argument, and uses it to generates the pdfs. 

It's written in pure python, and utilizes reportlab and pyqr. It's very fast (generated 2,845 pdfs in 45 seconds), and uses very little
resources. You can change the pdf by altering the text in the main.py file. 


You could easily modify this to your own needs. 
