# fun_shoping_discount.py
def discount(amount,member):
    disc=0
    if amount>=2000:
        disc=round((10+member)*amount/100,2)
    elif amount >=1000:
        disc=round((8+member)*amount/100,2)
    elif amount >=500:
        disc=round((5+member)*amount/100,2)
    payble=amount-disc        
    print("discount amount",disc)
    print("paybleamount:",payble)
amount=float(input("enter your shoping amount"))
member=input("is the customer a memeber?(Y/N)")
if member =="y"  or member=="Y":
    discount(amount,5)
else:
    discount(amount,0)    
