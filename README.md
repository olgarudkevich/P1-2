# P1-2

#Практична робота №1_2: Вказівники (Частина 1)

**Виконала:** студентка групи 4СОМ Рудкевич Ольга (Варіант № 2)

##  Завдання.

**Завдання:**
<img width="749" height="570" alt="image" src="https://github.com/user-attachments/assets/59c5d5dc-32b3-49a2-b158-76596883313b" />
<img width="657" height="20" alt="image" src="https://github.com/user-attachments/assets/dc96479a-8fc4-4a15-b53f-3c0b7ed2738b" />

<img width="227" height="20" alt="image" src="https://github.com/user-attachments/assets/0b296883-3d33-4c2b-a405-177e713f6e43" />

### 💻 Код програми:

#include <iostream>
2	
3	using namespace std;
4	
5	void updatePrice(double* pricePtr) {
6	    *pricePtr += 150; 
7	}
8	
9	int main() {
10	    //setlocale(LC_ALL, "Ukrainian");
11	
12	    int orderNumber = 205;
13	    int* ptr = &orderNumber;
14	
15	    cout << "--- Номер замовлення ---" << endl;
16	    cout << "Значення orderNumber: " << orderNumber << endl;
17	    cout << "Адреса &orderNumber: " << &orderNumber << endl;
18	    cout << "Адреса через вказівник ptr: " << ptr << endl;
19	    cout << "Значення через вказівник *ptr: " << *ptr << endl;
20	
21	    *ptr = 210; 
22	    
23	    cout << "Змінене значення orderNumber: " << orderNumber << endl << endl;
24	
25	    double weight = 4.8;
26	    double* weightPtr = &weight;
27	
28	    cout << "--- Основний параметр замовлення (вага) ---" << endl;
29	    cout << "Значення weight: " << weight << endl;
30	    cout << "Адреса &weight: " << &weight << endl;
31	    cout << "Адреса через вказівник weightPtr: " << weightPtr << endl;
32	    cout << "Значення через вказівник *weightPtr: " << *weightPtr << endl;
33	
34	    *weightPtr = 5.3;
35	    cout << "Змінене значення weight: " << weight << endl << endl;
36	
37	    double price = 950.0;
38	
39	    cout << "--- Вартість замовлення ---" << endl;
40	    cout << "Початкова вартість: " << price << " грн" << endl;
41	
42	    updatePrice(&price);
43	
44	    cout << "Нова вартість: " << price << " грн" << endl;
45	
46	    return 0;
47	}

### 👁️ Візуалізація пам'яті:

<img width="218" height="616" alt="image" src="https://github.com/user-attachments/assets/3bca9d02-43fb-47af-ac0f-2805792652c9" />


Фіксація скриншоту:

<img width="1130" height="738" alt="image" src="https://github.com/user-attachments/assets/6856f8fc-6e72-418a-b74f-3c211ee79b2b" />
