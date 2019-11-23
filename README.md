# Cplusplus11
版本 11 推出的功能

新功能：

1. 利用 constructor 建構 invariant （約束條件），並設計如失敗便可丟出 exception。

2. 利用 destructor 來簡化資源管理 （作者自問：換句話說，是指釋放資源嗎？）

3. 避免直接 new 和 delete 操作行為。

4. 利用容器 container 取代 內建 Array。

5. 利用 exception 例外錯誤處理機制取代局部處理錯誤。

6. 利用 move 搬移 取代 copy 複製（尤其是大型物件）。 

7. 所謂的共享物件，即 shared object，可以利用 shared_ptr 指向它們 （通常，此類物件沒有單一擁有者來負責 destruct 這共享物件）。

8. 避免強制轉型 cast ，可用 template 模板維護靜態型別的安全性。

9. 關於 polymorphic type 的物件，可以利用 unique_ptr 指向它們。

10. C++ 的 nested class 無法存取 enclosing class 外圍類別的物件。

題外話，給 Java 程式員的建議：

1) Style, 每種語言有各自風格，不恰當的混合使用風格，會導致可維護性低且效能無法達到最佳狀態。

2) Class, 無需為所有類別創建類別。

3) const, 使用區域變數與成員變數，避免使用指標變數或是參考的變數。

4) C++ 的參考變數無法重新指向，但 Java 可以...。

5) 獨立函數，即非成員函數，能 decouple 減少耦合關係。（撰寫獨立函數的方法，可利用命名空間與標準演算法。）

6) 一樣是釋放資源（清理動作，或是離開某作用域），finally 的維護成本比單純使用 destruct 高出許多。

7) 無論何時何地盡量使用 Scope 概念的 RAII, Resource Aquisition is Initialization, 資源獲取時即刻初始化。


