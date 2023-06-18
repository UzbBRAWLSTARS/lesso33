# lesso33
with open('amaliyot/pi_million_digits.txt') as file:
with open("amaliyot/pi_million_digits.txt") as file:
    pi = file.read()
pi = pi.rstrip() # qator ohiridagi bo'shliqlarni olib tashlaymiz
pi = pi.replace('\n','') # qator tashlash belgisini almashtiramiz
pi = pi.replace(' ','')
pi = pi.rstrip()  # qator ohiridagi bo'shliqlarni olib tashlaymiz
pi = pi.replace("\n", "")  # qator tashlash belgisini almashtiramiz
pi = pi.replace(" ", "")

# Tug'ilgan kunim pi da bormi?
bdate = '31122000'
bdate = "31122000"
print(bdate in pi)

while True:
    book = input("Yaxshi koʻrgan kitobingizni kiriting (to'xtash uchun Enter bosing): ")
    if not book: break
    with open('amaliyot/books.txt','a') as file:
        file.write(book+'\n')
    if not book:
        break
    with open("amaliyot/books.txt", "a") as file:
        file.write(book + "\n")
