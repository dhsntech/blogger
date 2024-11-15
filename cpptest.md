# 程式設計測驗練習(1~10)

### 1. 計算圓的周長和面積
```cpp
double ar;
cout << "輸入圓半徑:";
cin >> ar;
cout << "圓周長為:" << (ar * 2) * 3.14 << "\t圓面積為:" << (ar * ar) * 3.14;
```
- `double ar;` 定義了一個變數 `ar` 用來儲存圓的半徑。
- 使用 `cin >> ar;` 讓使用者輸入半徑的值。
- 圓周長公式是半徑乘以2再乘以3.14，而面積公式是半徑的平方再乘以3.14。
- `cout` 輸出計算結果。

### 2. 將秒數轉換成時、分、秒
```cpp
int bin, bs, bm, bh;
cout << "輸入秒數:";
cin >> bin;
bh = (bin / 60) / 60;
bm = (bin / 60) % 60;
bs = bin % 60;
cout << bh << "小時 " << bm << "分  " << bs << "秒  ";
```
- `bin` 是輸入的總秒數。
- 計算小時：`bh = (bin / 60) / 60;`
- 計算分鐘：`bm = (bin / 60) % 60;`
- 計算秒：`bs = bin % 60;`
- 最後 `cout` 輸出時、分、秒。

### 3. ASCII 值轉字元
```cpp
int ci;
char co;
cout << "輸入ASCII值:";
cin >> ci;
co = ci;
cout << "字元為:" << co;
```
- `int ci;` 用來儲存輸入的 ASCII 值。
- 將 `ci` 賦值給 `co`，這樣 `co` 就會變成對應的字元。
- `cout` 輸出字元。

### 4. 字元轉 ASCII 值
```cpp
char din;
int dout;
cout << "輸入字元:";
cin >> din;
dout = din;
cout << "ASCII值為:" << dout;
```
- `dout = din;` 取得 `din` 的 ASCII 值。
- `cout` 輸出 ASCII 值。

### 5. 攝氏轉華氏
```cpp
int ec, ef;
cout << "請輸入攝氏溫度:";
cin >> ec;
ef = ec * 9 / 5 + 32;
cout << "華氏溫度為:" << ef;
```
- 華氏溫度公式：`華氏 = 攝氏 * 9 / 5 + 32`。
- `cout` 輸出結果。

### 6. 判斷成績及格與否
```cpp
int fx;
cout << "請輸入成績:";
cin >> fx;
if (fx <= 100 && fx >= 0) {
    if (fx >= 60) {
        cout << "及格";
    }
    else if (fx < 60) {
        cout << "不及格";
    }
}
else {
    cout << "成績錯誤";
}
```
- 先判斷成績在 0 到 100 間。
- 如果成績大於等於 60，輸出「及格」，否則輸出「不及格」。

### 7. 判斷奇數或偶數
```cpp
int ix;
cout << "請輸入一個正整數:";
cin >> ix;
if (ix % 2 == 0) {
    cout << ix << "是偶數";
}
else {
    cout << ix << "不是偶數";
}
```
- 判斷 `ix` 除以 2 的餘數，若餘數為 0，表示偶數，否則是奇數。

### 8. 比較兩數大小
```cpp
int jx, jy;
cout << "請輸入第一個正整數a:";
cin >> jx;
cout << "請輸入第二個正整數b:";
cin >> jy;
if (jx == jy) {
    cout << "a等於b";
}
else if (jx > jy) {
    cout << "a大於b";
}
else if (jx < jy) {
    cout << "a小於b";
}
```
- 輸入兩個數 `jx` 和 `jy`，比較它們的大小。

### 9. 判斷兩數的奇偶性
```cpp
int kx, ky, ki = 0;
cout << "請輸入第一個正整數:";
cin >> kx;
cout << "請輸入第二個正整數:";
cin >> ky;
if (kx % 2 == 0) {
    ki++;
}
if (ky % 2 == 0) {
    ki++;
}
if (ki == 0) {
    cout << "兩個奇數";
}
else if (ki == 1) {
    cout << "一奇一偶";
}
else if (ki == 2) {
    cout << "兩個偶數";
}
```
- 根據 `ki` 的值來判斷兩數是否為奇數或偶數。

### 10. 判斷字元類型
```cpp
char lc;
int li;
cout << "輸入字元:";
cin >> lc;
li = lc;
if (li > 47 and li < 58) {
    cout << "數字";
}
else if (li > 64 and li < 91) {
    cout << "大寫字母";
}
else if (li > 96 and li < 123) {
    cout << "小寫字母";
}
else {
    cout << "無法辨識";
}
```
- 利用 ASCII 編碼範圍來判斷輸入字元是數字、大寫字母、小寫字母或其他。
