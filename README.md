# MessageBoardJS
Use JS to make the MessageBoard

6/6 00:06
格式化文件，讓程式碼好看點

6/5晚上11:26
嘗試使用DOM去動態增加結點
但還沒成功

6/4 晚上11:30
可以刪除指定留言
先以陣列去存每次輸入的值，每次輸入都是新的一個段落
可以刪除指定段落，看之後有沒有更好的做法

6/4 晚上10:50
輸入留言不蓋掉原本的留言

6/4 晚上7:30
發現如果使用addEventListener的話，應該用document去判斷
不應該
``` javascript=
const btn=document.getElementById
btn.addEventListener
```
如果是用onclick，必須在標籤裡就先做好
```html=
<input id="Save" onclick=save() type="button" value="儲存">
```
但目前不確定是不是這樣也不知道原因

6/3 晚上11:30
查詢可能可以透過getElementById去取buttion的id然後設定功能
但是實際寫上去沒有反應
想說試著用debugger下中斷點去測試，但是按按鈕後沒有進入debugger模式，不知該怎麼測試執行過程

6/3 晚上10:00
在家clone下來後發現中文變成亂碼
"可能"是因為透過notepad++開啟時，被預設編碼為ANSI
只能透過把亂碼改成中文後在push一次
還遇到了script 標籤 語法錯誤的問題，後來發現是因為把script寫在了style裡面，所以錯誤

6/3 白天
知道要在 <head> 標籤裡新增 script 標籤
現在已知需要讓btnSave可以有功能，但是不知script裡面該寫什麼

6/2
新增一個 <textarea> 當做輸入框
input 有 type="button" 的按鈕型態，id 為b tnSave
要做一個可以顯示留言的地方，但是想不到該用什麼標籤顯示比較好
就先新增了一個 <textarea> 把他的 readonly 屬性設為 readonly


- [x] 要有一個輸入框可以輸入留言
- [x] 要有一個顯示留言的地方
- [ ] 要有一個按鈕，按下後顯示留言的地方會有剛輸入的留言
