# LCTestsExample

## Unit test with XCTest

1. 驗證回傳
2. 驗證狀態改變
3. 驗證互動

### 3A原則
Arrange: 初始化
Act: 呼叫要測試的方法
Assert: 驗證結果

或者 Given / When / Then

## Naming

## TDD
1. 搞清楚spec
2. 設計接口(皮)與驗證方式
3. 最快方式填實作到綠燈

紅燈 > 綠燈 > 重構 loop

## Unit test and Integration test
- 外部依賴
任何存取到外部可能變動的來源都算是 Integration test，因為你的Code 沒改卻因為來源變動而造成Test fail
1. API
2. NSUserDefaults
3. File
4. DB
5. Singleton
6. NSDate

### 解除依賴
## 依賴注入 (dependency injection)
http://objccn.io/issue-15-3/
### 建構子注入 (構造器注入)
建議注入 id<xxxInterface>
如果注入太多參數，可能已經違背單一職能原則
### 屬性注入
### 方法注入


## (隔離框架) 把 Integration test 轉成 Unit test 
OCMock
1. Mock Method
2. Mock NSUserDefault
3. Mock Singleton


## 非同步測試
- Block
- NSNotification
- KVO

## UI testing - LoginViewController
1. 用 Category 暴露 private method

## TDD in production
