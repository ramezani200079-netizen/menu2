# menu2
name_list = []


while True:
    print("1)add name")
    print("2)show list")
    print("3)remove name")
    print("4)count name")
    print("0)exit")
    option = input("enter your option:")

    if option == "1":
        name = input("enter your name:")
        name_list.append(name)

    elif option == "2":
        print(name_list)


    elif option == "3":
        removed = input("enter your removed name:")

        if removed in name_list:
            name_list.remove(removed)
            print("removed successfully")

        else:
             print("the name was not in the list")

    elif option == "4":
        print(len(name_list))

    elif option == "0":
        print("exit")


    else:
        print("invalid option")
