

class Oyin:
    def komputer(self):
        import random
        qiyinchilik =  input("Qiyinchilikni tanlang:(*), (**), (***), (****), (*****)")
        if qiyinchilik =='*':
            print("Siz oson o'yinni tanladingiz\nTushuntirish: 1 va 50 sonlar oralig'i, 7 ta imkoniyat")
            urunish = 0
            tasodif = random.randint(1, 50)
            while True:
                son = int(input("Komputer oylagan sonni topishga harakat qilng>>>: "))
                if son==tasodif:
                    print("Topdiz")
                    break
                else:
                    if tasodif <son:
                        print("Katta son kiriting")
                        urunish +=1
                    elif tasodif >son:
                        print("Kichik son kiritdiz")
                        urunish +=1
                    if urunish ==7:
                        print(f"Urunishlar soni tugadi\nKomputer: {tasodif}")
                        break
        if qiyinchilik =='**':
            print("Siz ortacha o'yinni tanladingiz\nTushuntirish: 1 va 50 sonlar oralig'i, 4 ta imkoniyat")
            urunish = 0
            tasodif = random.randint(1, 50)
            while True:
                son = int(input("Komputer oylagan sonni topishga harakat qilng>>>: "))
                if son==tasodif:
                    print("Topdiz")
                    break
                else:
                    if tasodif <son:
                        print("Katta son kiriting")
                        urunish +=1
                    elif tasodif >son:
                        print("Kichik son kiritdiz")
                        urunish +=1
                    if urunish ==4:
                        print(f"Urunishlar soni tugadi\nKomputer: {tasodif}")
                        break
        if qiyinchilik =='***':
            print("Siz o'rtacha qiyin o'yinni tanladingiz\nTushuntirish: 1 va 100 sonlar oralig'i, 7 ta imkoniyat")
            urunish = 0
            tasodif = random.randint(1, 100)
            while True:
                son = int(input("Komputer oylagan sonni topishga harakat qilng>>>: "))
                if son==tasodif:
                    print("Topdiz")
                    break
                else:
                    if tasodif <son:
                        print("Katta son kiriting")
                        urunish +=1
                    elif tasodif >son:
                        print("Kichik son kiritdiz")
                        urunish +=1
                    if urunish ==7:
                        print(f"Urunishlar soni tugadi\nKomputer: {tasodif}")
                        break
        if qiyinchilik =='****':
            print("Siz qiyin o'yinni tanladingiz\nTushuntirish: 1 va 100 sonlar oralig'i, 5 ta imkoniyat")
            urunish = 0
            tasodif = random.randint(1, 100)
            while True:
                son = int(input("Komputer oylagan sonni topishga harakat qilng>>>: "))
                if son==tasodif:
                    print("Topdiz")
                    break
                else:
                    if tasodif <son:
                        print("Katta son kiriting")
                        urunish +=1
                    elif tasodif >son:
                        print("Kichik son kiritdiz")
                        urunish +=1
                    if urunish ==5:
                        print(f"Urunishlar soni tugadi \nKomputer: {tasodif}")
                        break
        if qiyinchilik =='*****':
            print("Siz eng qiyin o'yinni tanladingiz\nTushuntirish: 1 va 100 sonlar oralig'i, 4 ta imkoniyat")
            urunish = 0
            tasodif = random.randint(1, 100)
            while True:
                son = int(input("Komputer oylagan sonni topishga harakat qilng>>>: "))
                if son==tasodif:
                    print("Topdiz")
                    break
                else:
                    if tasodif < son:
                        print("Katta son kiritdiz")
                        urunish +=1
                    elif tasodif > son:
                        print("Kichik son kiritdiz")
                        urunish +=1
                    if urunish ==4:
                        print(f"Urunishlar soni tugadi\nKomputer: {tasodif}")
                        break

    def odam(self):
        import random
        a = 1
        b = 50
        urunish = 7
        while True:
            son = random.randint(a, b)
            son1 = input(f"{son} Siz oylagan son shumi To'gri(T), Katta(+), Kichik(-)").capitalize()
            if son1 == 'T':
                print("Toptim")
                break
            elif son1 == '+':
                a= son+1
                urunish-1
            elif son1 == '-':
                b = son-1
                urunish -=1
            if urunish ==0:
                print("Urunishlar soni tugadi")
                break
                
p = Oyin()
p.komputer()
