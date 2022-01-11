<h1> Recursion </h1>

<h2> Definations </h2>
    * It is a function calling it self until it reaches to some breaking or stopping conditions.

</br>
<h2> Properties </h2>
    * It has a charactaristic behaviour where it should call itself 
    * It has some breaking or stopping condition so that it cannnot goes into infinite state.
</br>

<h2> Iterative Vs Recrursion Approach to solve problem </h2>

![Screenshot 2022-01-10 at 4 02 56 PM](https://user-images.githubusercontent.com/52832896/148839389-408f0015-8c1c-4f2b-95ce-2c53d9591b5b.png)
</br>

<h2> When to use recursion and when to not </h2>
https://cestarcollege.adobeconnect.com/csd3354-4-week1/
</br>


few examples :
def sumofdigit(n):
    if(n == 0):
        return n
    else:
        return (int(n%10) + sumofdigit(int(n/10)))



print(sumofdigit(1293))


def powerofnumber(base, exp):
    if(exp==0):
        return 1
    else:
        return base * powerofnumber(base,(exp-1))

print(powerofnumber(2,7))


def gcdUsingEuc(n1,n2):
    if(n2 == 0):
        return n1
    else:
        return gcdUsingEuc(n2, int(n1%n2))

print(gcdUsingEuc(48,17))


def dectobin(n):
    if(int(n/2) == 0):
        return str(n)
    else:
        return  dectobin(int(n/2)) + str(int(n%2))

print(dectobin(13))
