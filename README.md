h=int(input("enter the height"))
r=int(input("enter the radius"))
f=int(input("enter the rate of flow"))
t=int(input("enter the time"))
volume=3.14*r**2
vrate=f*t
if vrate > volume:
        print("over flow condition")
        print("water overflowed",vrate - volume)
elif vrate == volume :
        print("tank full")
else:
        print("underflow condition")
        ht=vrate/(3.14*r**2)
        hr=h-ht
        print(f"filled height(ht)\n remaing height(hr)")
