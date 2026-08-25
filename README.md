# 이재우 (Jaewoo Lee)

게임 클라이언트 프로그래머를 목표로 하고 있습니다.
**Unity**와 **Unreal Engine**으로 개인 프로젝트를 만들면서, 기능을 붙이는 것보다
**나중에 고치기 쉬운 구조로 만드는 것**에 관심을 두고 공부하고 있습니다.

- 🔧 C++ · C# / Unreal Engine 5 · Unity 6
- 🌐 멀티플레이(Photon PUN2, UE 리플리케이션), 백엔드 연동(Unity Gaming Services)
- ✍️ 블로그 — https://blog.naver.com/apple_mango7228

---

## 대표 프로젝트

### [니벨아레나 (NivelArena)](https://github.com/apppleManGO/NivelArena-showcase) · Unity 6 · 1인
TCG 룰을 구현한 개인 프로젝트. 카드 804종 · 효과 700여 종 · 온라인 대전 · 계정 기반 클라우드 덱 저장.

싱글 플레이로 완성한 뒤 온라인 대전을 추가해야 했는데, 카드 효과가 모두 단독 실행을 전제로
작성되어 있었습니다. 효과마다 네트워크 분기를 넣는 대신 **모든 '행동'과 '선택'을 단일 진입점으로
수렴**시키고 그 아래에 네트워크 경계를 두어, **기존 게임 로직 수정 없이** 온라인 대전을 추가했습니다.
같은 구조를 이후 계정·클라우드 저장 기능에도 그대로 재사용했습니다.

> 실존 TCG의 룰을 개인 학습 목적으로 구현했습니다. 카드 이미지와 카드 데이터는 원저작자의
> 자산이므로 저장소에서 제외했고, 직접 작성한 코드와 설계 문서만 공개합니다.

### [던전구출자 (Dungeon Rescuer)](https://github.com/apppleManGO/Dungeon_Rescuer) · UE5.4 · 1인
멀티플레이어 협동 액션. 로비 상태·캐릭터 스킨 네트워크 동기화, 서버 권한 기반 상호작용,
씬 전환 시 상태 보존을 구현했습니다.

처음 완성한 뒤 시간을 두고 다시 읽어보며 구조를 정리하는 리팩토링을 진행했습니다.

### [숲에서 살아남기 (TurnBasedTileTactics)](https://github.com/apppleManGO/TurnBasedTileTactics) · UE5.4 · 1인
턴제 전략 시뮬레이션. 그리드 기반 이동과 턴 관리, 하나의 키로 이동·조준을 전환하는
상태 기반 입력 처리, 타겟 추적 AI를 구현했습니다.

### [원소울 (One Soul)](https://github.com/normalnine/OneSoul_5_0) · UE5.0 · **3인 팀**
다크 소울을 레퍼런스로 한 3D 액션 RPG. **플레이어 전투 시스템(회피·가드)과 몬스터 AI**를 맡았습니다.

구르기를 물리 임펄스(`AddImpulse`)로 구현했더니 캐릭터가 미끄러지고 벽에 박히는 문제가 있었습니다.
매 틱 방향 벡터를 계산해 위치를 직접 갱신하는 방식으로 바꾸고 콜리전을 조정해,
외부 환경에 영향받지 않는 조작감을 만들었습니다.

> 팀 프로젝트이며, 저장소는 팀원 계정에 있습니다.

---

## 학습 기록

- [GameClientStudyNotes](https://github.com/apppleManGO/GameClientStudyNotes) — 게임 클라이언트 개발 학습 정리
- 블로그에 프로젝트를 만들며 겪은 문제와 해결 과정을 남기고 있습니다 — https://blog.naver.com/apple_mango7228
