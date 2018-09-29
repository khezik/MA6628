# MA6628
#Prj01
def is_prime(n):
   for i in range(2, n):
      if n % i == 0:
         return False
   return True

def generate_twins(start, end):
   a = 0
   for i in range(start, end):
      j = i + 2
      if j in range(start,end):
          if(is_prime(i) and is_prime(j)):
             a = a+1
   return a
