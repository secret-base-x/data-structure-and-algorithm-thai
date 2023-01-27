# Data Structure และ Algorithm ในภาษาไทย


# Data Structure

## Data Structure คืออะไร
- ในทาง Computer Science นั้น Data Structure เป็นรูปแบบการจัดการ บริหาร และจัดเก็บข้อมูลที่สามารถ **เข้าถึงและแก้ไข** ข้อมูลอย่าง **มีประสิทธิภาพ**

## ทำไม Data Structure ถึงเป็นสิ่งจำเป็น
- Data Structure แต่ละแบบทำให้เราสามารถจัดเก็บข้อมูลในรูปแบบที่แตกต่างกันได้
- ทำให้สามารถ**ค้นหา**ข้อมูลและ**ดึง**ข้อมูลได้อย่าง**มีประสิทธิภาพ**
- Data Structure ในแต่ละรูปแบบเหมาะกับการแก้ปัญหาเฉพาะด้านที่แตกต่างกัน
- Data Structure ช่วยทำให้เราจัดการข้อมูลขนาดใหญ่อย่างฐานข้อมูลได้ หรือระดับดัชนีข้อูลเช่น (Indexing) เช่น Hash Table
- เน้นที่ค้นหาและดึงข้อมูลได้อย่างมีประสิทธิภาพ เหมือนการเก็บของในห้อง แค่โยนๆ เข้าไปในห้องก็คือการเก็บแล้ว แต่ทำยังไงล่ะ ถึงเป็นการต้นหาและจัดเก็บข้อมูลได้อย่างมีประสิทธิภาพ
- เทีบบกับในชีวิตประจำวัน การค้นหาคำศัพท์ใน Dictionary สามารถค้นหาได้ง่าย เพราะมันเรียงตามตัวอักษร ในระบบของ Data Structure ของโลกดิจิตอลก็เป็นแบบนีั้น
- ในแผนที่ถ้าเราต้องการเก็บข้อมูลเป็น Location ก็อาจจะเก็บเป็น X,Y นี่ก็เป็นตัวอย่างของการเก็บข้อมูล
- การจัดเก็บข้อมูลใน Excel ที่เก็บเป็นรูปแบบตารางแบบ Row และ Column และสามารถหาจำนวนมากสุดได้ หาค่าเฉลี่ยได้ เป็นอีกตัวอย่างนึงของ Data Structure

## Array 
- Array โครงสร้างข้อมูลประเภทเดียวกัน (เช่น Int, String) ที่ถูกมัดรวมไว้เป็น Collections มี Address ที่ติดๆ กันใน RAM สามารถอ้างถึงแต่ละอันได้ด้วย Index
- Array เป็นหนึ่งในรูปแบบของ Data structure ที่พื้นฐานที่สุด
- ในภาษาโปรแกรมมิ่งจำนวนมากก็มักจะมี Array มาให้ใช้งานอยู่แล้ว
- พวกโครงสร้างข้อมูลอย่าง Stack, Queue, Graph แบบนี้เราต้องมี Implement เอาเองแต่ Array นี่คือมีให้มาอยู่แล้วตั้งแต่ระดับของภาษาโปรแกรมมิ่ง



```cpp
#include <iostream>
#include <cstdlib>

int main() {
    int myArray[4] = {1, 2, 3, 4};

    for (int i = 0; i < 4; i++) {
        std::cout << "Memory address of myArray[" << i << "]: ";
        std::cout << &myArray[i] << " (base 16) "; // cast the address to unsigned long to print it as hexadecimal
        std::cout << (unsigned long)&myArray[i] << " (base 10)" << std::endl;
    }
    return 0;
}
```

```zsh
Memory address of myArray[0]: 0x16f93f590 (base 16) 6166934928 (base 10)
Memory address of myArray[1]: 0x16f93f594 (base 16) 6166934932 (base 10)
Memory address of myArray[2]: 0x16f93f598 (base 16) 6166934936 (base 10)
Memory address of myArray[3]: 0x16f93f59c (base 16) 6166934940 (base 10)
```

จากตัวอย่างนี้จะพบว่าตำแหน่งใน Memory (หน่วยความจำ) ใยฐาน 10 จะต่างกันที่ละ 4 ต่อ Index เพราะ Int ใช้พื้นที่หน่วยความจำ 4 bytes โดย 1 Memory Location นั้นจะเก็บ 1 Byte (8 Bits)

การที่ตำแหน่งของข้อมูลในหน่วยความจำอยู่ติดกัน ทำให้การเข้าถึง Index ที่ต้องการสามารถเข้าถึงได้ง่ายเร็วและสะดวก

# แหล่งข้อมูล
[Youtube Playlist เรื่อง Data Structure and Alogrithm ของช่อง Simple Snippets](https://www.youtube.com/playlist?list=PLIY8eNdw5tW_zX3OCzX7NJ8bL1p6pWfgG)
