Apple의 대표적인 IDE인 Xcode의 프로젝트 생성 과정을 알아보았다.

## Xcode 설치 및 설정
Xcode는 공홈 또는 앱 스토어에서 다운을 받을 수 있다.

1. 웹 페이지
![](https://velog.velcdn.com/images/kimjaewoo522/post/2efeeb13-86ff-493c-afe8-3c82ad639524/image.png) (https://developer.apple.com/kr/xcode/resources/)


2. 앱 스토어
![](https://velog.velcdn.com/images/kimjaewoo522/post/66af3ace-d204-4bbe-b192-504bfd9c7a5c/image.png)


## 새로운 프로젝트 생성
1. Xcode 실행
	- "Create a new Xcode project"를 클릭하거나, 상단 메뉴에서 File > New > Project를 선택하면 된다.
![](https://velog.velcdn.com/images/kimjaewoo522/post/1f40b1b6-965b-4903-b16b-6d043b9767b6/image.png)

2. 플랫폼 및 템플릿 선택

- 나타나는 창에서 앱을 실행할 운영체제(iOS, macOS, watchOS 등)를 선택한다

- 앱 유형을 선택한다(예: Single View App, 게임 증강 현실앱 등)

![](https://velog.velcdn.com/images/kimjaewoo522/post/27f6809b-cb43-4d55-a257-390da8096092/image.png)

3. 프로젝트 옵션 입력
- Product Name 입력
- Organization Identifier 입력
**_Organization Identifier란?_** : 이 값은 Bundle Identifier(번들 ID)를 생성하는 데 사용되며, Xcode 프로젝트를 만들 때 필수적으로 입력
- Organization Name 입력 or 본인 이름 입력
- Language : 사용할 프로그래밍 언어 선택(Swift or Objective-C)
- User Interface : SwiftUI, Watchkit, UIKit, AppKit, TVUIKit 등 중에 선택

![](https://velog.velcdn.com/images/kimjaewoo522/post/65913369-02f4-4aaf-a0af-ca779d63a4d1/image.png)

4. Next를 누르면 생성 완료!

이를 통해 Xcode의 프로젝트를 생성하는 법을 알게 되었다.

**참고**

- https://developer.apple.com/documentation/xcode/creating-an-xcode-project-for-an-app
