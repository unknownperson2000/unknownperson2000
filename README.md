string_n= "Tea:0.50,Cola:0.33,Cake:1.00,Chips:0.65"
v=['0','1','2','3','4','5','6','7','8','9']
h=[]
c=[]
i=0
while(i+1<len(string_n)):
  if string_n[i] in v :
    if string_n[i+1] =='.':
      c.append(string_n[i])
      c.append(string_n[i+1])
      c.append (string_n[i+2])
      c.append (string_n[i+3])
      q = ''.join([str(elem) for elem in c])
      i=i+3
      h.append(float(q))
    else :
      h.append(float(string_n[i]))
  c.clear()
  i=i+1
print(h)
print(sum(h))
'''string_n = "Tea:0.50,Cola:0.33,Cake:1.00,Chips:0.65"
v = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']
h = []
c = []
i = 0
while (i + 1 < len(string_n)):
    if string_n[i] in v:
        if string_n[i + 1] == '.':
            c.append(string_n[i])
            c.append(string_n[i + 1])
            c.append(string_n[i + 2])
            c.append(string_n[i + 3])
            q = ''.join([str(elem) for elem in c])
            i = i + 3
            h.append(float(q))
        else:
            h.append(float(string_n[i]))
    c.clear()
    i = i + 1
print(string_n)
separator = ","
print(separator.join(string_n))
print(sum(h))'''
# the second one deals with separator to show all the chars in the string .. you may delete the triple quotation and try it
#you can replace the string with anything and it will count it and find the process of adding numbers
