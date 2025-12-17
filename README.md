
    print("===欢迎来到糖心猜数字===")
    print("请输入1~100的一个整数")
    import random
    draws = 0
    randnum = random.randint(1,100)
    while True:
        try:
            draws += 1
            yournum = int(input("请猜一猜这个数是："))
            if yournum == randnum:
                print(f"恭喜你！猜对了！这个数就是{randnum}！你一共尝试了{draws}次！")
                break
            elif 100 >= yournum > randnum >=1:
                print("哥哥，太大了！")
            elif 1<= yournum < randnum <=100:
                print("弟弟，太小了！")
        except ValueError:
            print("妈的，请输入1~100的一个整数！")
