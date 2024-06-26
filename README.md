
# 자바로 만든 오델로 게임

## 소개
이 프로젝트는 자바를 사용하여 고전 보드 게임 오델로(리버시)를 구현한 것입니다. 오델로는 두 명의 플레이어가 8×8 격자 보드에서 경쟁하는 전략 보드 게임입니다. 목표는 마지막으로 플레이 가능한 빈 칸이 채워졌을 때 자신의 색깔이 표시된 디스크가 가장 많도록 하는 것입니다.

## 팀원
- 박나현
- 이승재

## 기능
- **단일 플레이어 vs. AI**: AI를 상대로 게임을 플레이할 수 있습니다.
- **2인용 모드**: 두 명의 플레이어가 번갈아 가며 게임을 진행할 수 있습니다.
- **게임 규칙 적용**: 오델로의 모든 규칙이 정확하게 구현되었습니다.
- **실시간 점수 표시**: 각 턴마다 현재 점수를 실시간으로 확인할 수 있습니다.
- **유효한 이동 표시**: 현재 턴에서 가능한 모든 유효한 이동을 표시해줍니다.

## 설치 및 실행 방법
1. 저장소를 클론합니다:
    ```bash
    git clone https://github.com/yourusername/othello-game.git
    ```
2. 프로젝트 디렉토리로 이동합니다:
    ```bash
    cd othello-game
    ```
3. 프로젝트를 빌드하고 실행합니다:
    ```bash
    javac -d bin src/*.java
    java -cp bin Main
    ```

## 게임 방법
1. 게임을 시작하면 초기 보드가 표시됩니다.
2. 두 플레이어는 번갈아 가며 자신의 디스크를 놓습니다.
3. 디스크를 놓을 때마다 상대방의 디스크를 뒤집을 수 있는 위치에만 놓을 수 있습니다.
4. 게임이 끝나면 더 많은 디스크를 가진 플레이어가 승리합니다.

## 프로젝트 구현 방식
- **Board.java**: 돌을 둘 수 있는 자리 탐색, 돌 뒤집기, 보드판 초기화 등을 실행합니다.
- **BoardPanel.java**: 이벤트 처리를 통해 각 단계에 대한 안내창을 생성합니다.
- **ComputerPlayer.java**: 보드판의 자리 우선순위에 대한 점수를 지정해 AI가 최적의 자리에 돌을 놓도록 계산합니다.
- **OthelloApp.java**: 메인 메소드를 포함하고 있으며, 이벤트 처리를 통해 게임의 메인 화면을 생성합니다.
- **Stone.java**: 돌에 관련된 함수들을 선언합니다.

## 프로젝트 후기
Java 언어로 진행하는 첫 프로젝트로, GUI를 만들어 결과를 확인하는 것이 유익한 경험이었습니다. 하지만 몇 가지 아쉬운 점도 있었습니다. 게임 안내문의 닫기 버튼이 제대로 작동하지 않고, 사용자의 별명을 입력받지만 적용되지 않으며, socket과 thread를 이용한 클라이언트 간 게임 구현에 실패한 점 등이 있습니다. 

## 발표 영상
[발표 영상 보기](https://www.youtube.com/watch?v=i0AVsR4GVPo)
