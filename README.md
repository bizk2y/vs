# Visual Studio

## Visutal Studio 설치 

참조 [명월일지](https://nowonbun.tistory.com/68 "Visuatl Studio 설치하는 방법")

1. https://visualstudio.microsoft.com/vs 에 접속하여 Community버전을 다운로드 받는다.
2. 설치 파일을 클릭해서 실행하면 설치에 필요한 파일을 설치한다.
3. 설치가 끝나면 이제 설치 옵션에 대한 메뉴가 나온다.
   - ASP.NET, Python, .Net Desktop, C++을 설치한다.
   - 설치 후 필요한 컴포넌트가 있으면 추가로 설치할 수 있다.
4. 설치가 완료되면 로그인 메뉴가 나오는데, Microsoft 아이디를 넣고 로그인을 한다.
   - 로그인을 하지 않으면 Community도 30일만 사용할 수 있다.
5. 로그인을 하고 나면 프로젝트를 선택하는 화면이 나옵니다. 일단 제대로 설치가 되었는지 확인하기 위해서 "새 프로젝트 만들기(N)"을 선택한다.
6. 새 프로젝트 만들기
   1. C# 콘솔 프로젝트를 선택합니다. 여기서 Core 버전이 아닌 .NET Framework를 선택합니다.
      - 모든 언어: C#
      - 모든 플랫폼: Windows
      - 모든 프로젝트 형식: 콘솔
      - 콘솔 앱(.NET Framework)
7. 새 프로젝트 구성  
   - 프로젝트 이름과 위치를 입력한다.
   - 솔루션 및 프로젝트를 같은 디렉터리에 배치(D) 체크
8. 환경 설정
   - 도구(T) > 옵션(O)에서 환경 > 색 테마(C)를 어둡게 설정한다.
9. 테스트 소스 작성
    ``` c
    using System;
    using System.Collections.Generic;
    using System.Linq;
    using System.Text;
    using System.Threading.Tasks;

    namespace HelloWorld
    {
        class Program
        {
            static void Main(string[] args)
            {
                // 콘솔 출력
                Console.WriteLine("Hello World!");
                // 아무키나 눌러주세요.
                Console.WriteLine("Press Any Key ...");
                Console.ReadKey();
            }
        }
    }
    ```
10. F5버튼을 눌러 빌드한다.

## Visual Studio와 GitHub 연동하기

1. GitHub 원격 저장소 생성
2. Visual Studio에 GitHub Extension 설치
   1. 확장 > 확장 관리
   2. "GitHub Extension for Visual Studio" 설치한다.
   3. Visual Studio를 끄면 설치를 시작한다.
3. 저장소 복제
   1. 재시작 후 "팀 탐색기" 창을 열어보면 "호스티드 서비스 공급자"에 "GitHub"이 추가된 것을 확인할 수 있다.
   2. "연결..."을 클릭해 GitHub에 로그인 합니다. 성공적으로 연결이 되면 "팀 탐색기"에 "GitHub"이 추가된다.
   3. 이미 Git 원격 저장소가 있다면 "복제"를, 원격 저장소를 새로 만들려면 "만들기"를 클릭한다.
   4. 사용할 저장소를 선택 한 후 로컬 경로를 지정합니다. 이후 "복제"버튼을 클릭한다.
   5. 복제에 성공하면 "팀 탐색기"에서 좌측과 같은 화면을 확인할 수 있다.
4. 솔루션 생성 및 Commit
   > 팀 탐색기 -> 솔루션 -> 새로 만들기를 선택해 솔루션을 생성한다.
   1. 솔루션을 생성한 후 "프로젝트"의 "변경 내용"을 선택한다.
   2. 커밋 메시지를 입력한다. 하단의 변경내용을 확인한 후 "모두 커밋" 버튼을 클릭해 커밋 작업을 수행한다.
   3. 만약 해당 변경 내용을 바로 원격서버에 푸시하고 싶다면 "모두 커밋" 버튼의 삼각형을 눌러 "모두 커밋 후 푸시"를 선택합니다.




