# Discount-Coupon
cno=int(input('Enter Customer Phno:'))
cadd=input('Enter Address:')
coupon=input('Enter coupon code:')
bill=int(input('Enter total bill:'))
if bill>3000:
    tax=bill*15/100
elif bill>2000:
    tax=bill*10/100
elif bill>1000:
    tax=bill*7/100    
elif bill>500:
    tax=bill*5/100
else:
    tax=100
if coupon=='DIWALI':
    if bill>5000:
        dis=bill*10/100
    elif bill>3000:
        dis=bill*6/100
    elif bill>1000:
        dis=bill*4/100
    else:
        dis=0    
if coupon=='CHRISMAS':
    if bill>3000:
        dis=bill*20/100
    elif bill>2000:
        dis=bill*10/100
    elif bill>1000:
        dis=bill*5/100
    else:
        dis=0
print('Customer Name:',cname)
print('Customer Phno:',cno)
print('Customer Address:',cadd)
print('Tax is',tax)
print('Discount is',dis)
bill=bill+tax-dis
print('Total Amount is',bill)
