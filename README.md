# ambikeshsingh_HiiLoGame
This is HiLo Game- guessing number game
user guess number between 1 to 1000.
Program guess number given by User.


***************************************
***************************************

low=1
high=1000
print("Please ENTER number between {} to {} : ".format(low,high))
input("Please Enter Number  ")
guesses=1
while True:
    guess=low+(high-low)//2
    high_low=input("My guess is {}. Should I guess Highr or Lower ? "
                   "Enter h or l or ,c if my guess was correct   :".format(guess)).casefold()
    if high_low=="h":
        low=guess+1
    elif high_low=="l":
        high=guess-1
    elif high_low=="c":
        print("Bingoo")
        print("I got {} guessess ".format(guesses))
        
        break
    else:
        print("Plese enter h,l or c  ")
    guesses=guesses+1


