# js-lab-38
### Lab38 Conditiona: Guess Result13
คำสั่ง alert ในแต่ละบรรทัดจะแสดงค่าเป็นอะไรบ้าง   
หริณ มาเบ้า

```JavaScript
alert(null || 2 || undefined);
alert(alert(1) || 2 || alert(3));
alert(1 && null && 2);
alert(alert(1) && alert(2));
alert(null || (2 && 3) || 4);
```

```Shell
result
alert(null || 2 || undefined); -----> แสดงค่า 2 
alert(alert(1) || 2 || alert(3)); -----> แสดงค่า 1(alert1 เป็น undifined มีค่า false จึงแสดงตัวถัดไป) แล้วก็ 2(2 เป็นค่า true ตัวแรกจึงไม่แสดงตัวถัดไป)
alert(1 && null && 2); -----> แสดงค่า  null เพราะ null เป็น false ตัวแรก
alert(alert(1) && alert(2)); -----> แสดงค่า 1 และ undifined(ทำการ alert 1 ก่อน จึงคืนค่าของ alert ออกมาเป็น undefined)
alert(null || (2 && 3) || 4); -----> แสดงค่า  3 ( 2 && 3 คืนค่า 3 เพราะ && คืนค่า true ตัวสุดท้าย)
```

