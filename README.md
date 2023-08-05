# Caesar-cipher
Caesar-cipher encoded and decoded 
alphabet = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z', 'a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z']

direction = input("Type 'encode' to encrypt, type 'decode' to decrypt:\n")
text = input("Type your message:\n").lower()
shift = int(input("Type the shift number:\n"))

def encrypt(plain_text, shift_amount):
  cipher_text = ""
  for letter in plain_text:
    position = alphabet.index(letter)
    new_position = position + shift_amount
    cipher_text += alphabet[new_position]
  print(f"The encoded text is {cipher_text}")

  new_text =""
  for letter in input_text:
    position_letter = alphabet.index(letter)
    new_position = position_letter - shift_no
    new_letter = alphabet[new_position]
    new_text += new_letter
  print(f"Decrypt code is {new_text}")

if direction == "encode":
  encrypt(plain_text=text, shift_amount=shift)
elif direction =="decode":
  decrypt(input_text=text, shift_no=shift)
else:
  print("WTF")
