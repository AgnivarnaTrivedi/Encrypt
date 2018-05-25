# Encrypt
Basic encryption code in python

letters = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
encryption_code = 'LFWOAYUISVKMNXPBDCRJTQEGHZ'
letters += letters.lower()
encryption_code += encryption_code.lower()
enc = dict(zip(letters,encryption_code))

dec = dict(zip(encryption_code, letters))


s=input()

encr = "".join([enc.get(ch, ch) for ch in s])
decr = "".join([dec.get(ch, ch) for ch in encr])

print(encr)
print(decr)
