# ConySwiftUITutorials
https://developer.apple.com/tutorials/swiftui/creating-and-combining-views  학습하기 위한 저장소

## Section 1

### 새 프로젝트 만들기 및 캔버스 탐색

1. Xcode를 열고 Create a new Xcode project 
2. Single View App 클릭
3. 프로젝트 이름을 주고, User Interface : SwiftUI 클릭
4. ContentView.swift 파일 클릭
5. 캔버스가 보이지 않으면 **Editor > Canvas** 선택한다. 캔버스에서 **Resume** 클릭하여 미리보기를 표시한다.
6. View body 속성에서 코드를 변경하면 변경 사항을 반영하도록 미리보기가 업데이트 된다.



## Section 2

### 텍스트보기 사용자 정의

코드(code)를 변경하거나 인스펙터(inspector)를 사용하여 변경한다.

### inspector

- 캔버스의 미리보기에서 Command 버튼을 누르고 클릭하면, Show SwiftUI Inspector... 클릭
- Inspector로 수정(modifier)을 하다가 처음 상태로 돌아가고 싶으면 Command 버튼을 누르고 클릭하고 Show SwiftUI Inspector... 클릭하고, 예를 들어) 글자색을 변경하였다면 -> 색상 팝업 메뉴를 클릭하고 상속(**Inherited**)를 선택하면 수정(modifier)한것이 제거가 된다.
- 



### code

- 직접 코드로 추가한다. (삭제시 코드를 제거한다.)

```swift
import SwiftUI

struct ContentView: View {
    var body: some View {
        Text("Turtle Rock")
            .font(.title)
            .foregroundColor(.green)
    }
}

struct ContentView_Preview: PreviewProvider {
    static var previews: some View {
        ContentView()
    }
}
```



## Section 3

### 스택을 사용하여 뷰 결합

