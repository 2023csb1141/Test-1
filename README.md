# Oceanverse -59
# Caeser cipher
def encrypt(a) :
    alp="abcdefghijklmnopqrstuvwxyz"
    b=""
    for i in a :
        if i=="z" :
            b= b+"a"
        elif i==" " :
            b= b+" "
        else :
            b= b+alp[alp.index(i)+1]
    return b

def main() :
    a= input("Enter the message you want to encrypt: ")
    print(encrypt(a))
    
main()
