# Cplusplus11
版本 11 推出的功能

新功能：

1. 利用 constructor 建構 invariant （約束條件）。

2. 利用 destructor 來簡化資源管理 （作者自問：換句話說，是指釋放資源嗎？）

3. 避免直接 new 和 delete 操作行為。

4. 利用容器 container 取代 內建 Array。

5. 利用 exception 例外錯誤處理機制取代局部處理錯誤。

6. 利用 move 搬移 取代 copy 複製（尤其是大型物件）。 

7. 所謂的共享物件，即 shared object，可以利用 shared_ptr 指向它們 （通常，此類物件沒有單一擁有者來負責 destruct 這共享物件）。

8. 避免強制轉型 cast ，可用 template 模板維護靜態型別的安全性。

9. 關於 polymorphic type 的物件，可以利用 unique_ptr 指向它們。
