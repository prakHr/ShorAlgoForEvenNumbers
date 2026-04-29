# URL :- [https://pypi.org/project/my-shor-package/4.0.0/]

# ShorAlgoForEvenNumbers
contains solution of uncrackable shor's algorithm using data structures and parallel processing


    NEWLINE_CHAR = "\n"
    for string in ["4","6","10","19","9992","999999992","1234","1234567898"]:
        # print(string)
        out = parallel_for_loop_factor(int(string))
        print(f"Factors of {string} using for loop: {out}")
        print(NEWLINE_CHAR)

    for string in ["2"*10,"2"*20,"2"*50,"2"*100,"2"*200]:
        print(len(string))
        fast_out = parallel_for_loop_factor(int(string))
        print(f"Factors of {string} using parallel for loop: {fast_out}")
        print(NEWLINE_CHAR)
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

    for length in [10, 11, 12, 13, 14, 15, 16]:
        string = ""
        for i in range(1, length+1):
            string += str(9)
        n=len(string)
        if int(string[n-1])%2==1:
            string = string[:-1] + "2"
        print(string)
        print(len(string))
        fast_out = parallel_for_loop_factor(int(string))
        print(f"Factors of {string} using parallel for loop: {fast_out}")

        print("\n\n")

    for length in [20]:
        string = ""
        for i in range(1, length+1):
            string += str(9)
        n=len(string)
        if int(string[n-1])%2==1:
            string = string[:-1] + "2"
        print(string)
        print(len(string))
        fast_out = parallel_for_loop_factor(int(string))
        print(f"Factors of {string} using parallel for loop: {fast_out}")

        print("\n\n")
    
    string = "11"
    print(string)
    out = parallel_for_loop_factor(int(string))
    print(f"Factors of {string} using for loop: {out}")

    length = 100
    string = ""
    for i in range(1, length+1):
        string += str(random.randint(1,9))
    n=len(string)
    if int(string[n-1])%2==1:
        string = string[:-1] + "1"
    print(string)
    print(len(string))
    fast_out = parallel_for_loop_factor(int(string))
    print(f"Factors of {string} using parallel for loop: {fast_out}")
