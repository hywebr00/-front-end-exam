## 凌網科技股份有限公司研究發事業處：前端工程師徵才試題 🚀

我們是台灣圖書館電子書第一品牌 HyRead 的研發團隊，歡迎有自信、對軟體開發充滿熱情的夥伴加入，一同發掘數位閱讀的無限可能。

### 1. 流程

1. 請自行建立 **React** 專案
2. 這裡有一個基礎 [Figma](https://www.figma.com/file/4aAUNkjFEd8q5RF1zbzCrI/HyRead?node-id=0%3A1&t=bQdnfIBB6eyN68zn-1) 設計稿 👋
3. 請您盡可能的建立一個**好的架構 (如果是 Redux 更好）**、**乾淨的代碼** ✨
4. **實作服務請求**👇拿到『使用者書單』資料 📕
5. 必須要有可以**收藏**與**取消收藏** ❤️
6. 將您完成好的專案上傳至您個人的 **Github**
7. **郵件**您的**存儲庫 (Repository) 連結**以及您個人的**履歷、面試資料**等至 HR: *wendy@hyweb.com.tw*
8. 符合標準將會通知您來進行**面試**
9. 其他問題可詢問公司 **HR 李小姐: (02)2395-6966 #3128**

<br>

> **額外加分**
> 1. 整合 **RxJS** 加分 👍
> 2. 整合 **Redux-observable** 加分 👍
> 2. 盡可能地將 **您會的技術實作出來** 加分 👍

<br>

### 2. 服務串接

- **URL:**
    **`GET`**  https://mservice.ebook.hyread.com.tw/exam/user-list

- **Request header:**
    | header|  value|
    |:--:|:--:|
    |Content-type| application/json|

- **Response:**
    | 欄位|  說明|
    |:-----:|:-----:|
    |uuid |  唯一碼 |
    |coverUrl |  書封圖片 |
    |publishDate |  出版日期 |
    |publisher |  出版社 |
    |author |  作者 |

```json
[
  {
    "uuid": 0,
    "title": "藍色時期. 7",
    "coverUrl": "https://webcdn2.ebook.hyread.com.tw/bookcover/270374978957267916620215022111051.jpg",
    "publishDate": "2021[民110]",
    "publisher": "東立出版社",
    "author": "山口飛翔 著"
  },
  {
    "uuid": 1,
    "title": "[試讀本] 熾熱之夢",
    "coverUrl": "https://webcdn2.ebook.hyread.com.tw/bookcover/278194978986319625920223411010153.jpg",
    "publishDate": "2022[民111]",
    "publisher": "蓋亞文化",
    "author": "喬治.馬汀著;章澤儀譯"
  },
  /// 省略
]
```
