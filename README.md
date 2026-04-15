# ShorAlgoForEvenNumbers
contains solution of uncrackable shor's algorithm using data structures and parallel processing


    string = "2"*10
    print(string)
    out = parallel_for_loop_factor(int(string))
    print(f"Factors of {string} using for loop: {out}")

    string = "2"*200
    print(len(string))
    fast_out = parallel_for_loop_factor(int(string))
    print(f"Factors of {string} using parallel for loop: {fast_out}")

    length = 100
    string = ""
    for i in range(1, length+1):
        string += str(random.randint(1,9))
    n=len(string)
    if int(string[n-1])%2==1:
        string = string[:-1] + "2"
    print(string)
    print(len(string))
    fast_out = parallel_for_loop_factor(int(string))
    print(f"Factors of {string} using parallel for loop: {fast_out}")
