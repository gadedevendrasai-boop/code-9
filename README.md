# code-9
password strength checker &amp; factor machine production

password=input()
specials={"@","#","$","&","!","*"}
has_upper=any(c.isupper()for c in password)
has_lower=any(c.islower()for c in password)
has_digit=any(c.isdigit()for c in password)
has_special=any(c in specials for c in password)
if has_upper and has_lower and has_digits and has_special:
    print("Stron password")
  else:
      print("Not strong")


n=int(input())


found = False
for i in range(1,n+1):
    val = int(input())
    if val < 50 and not found:
        print(i)
        found = True


if not found:
    print("Stable")
