# BossSoul3

『다크 소울 3』의 보스전을 모작한 3인칭 소울라이크 액션 게임

**Unreal Engine 5** · Blueprint<br>
UE 클라이언트 2인 · 개발 기간 4주
# 보스소울3 (BossSoul3)

『다크 소울 3』의 보스전을 모작한 3인칭 소울라이크 액션 게임

**Unreal Engine 5.6** · Blueprint<br>
UE 클라이언트 2인 · 개발 기간 4주

[시연 영상](https://youtu.be/cnK2GnQKoQM) · [상세 기술 문서](https://app.notion.com/p/3-349e6578029f803ca997ca90b28f1e71)

## 게임 소개

반복된 죽음으로 패턴을 익혀 보스를 공략하는 소울라이크 보스전입니다.
정확한 타이밍의 패링으로 보스를 그로기 상태에 빠뜨려 치명타를 노리고,
화톳불에서 회복하며 다시 도전하는 흐름을 구현했습니다.
높은 난이도의 보스 AI와 정교한 전투 판정으로 도전과 성취감을 목표로 했습니다.

## 주요 구현

**플레이어 캐릭터 · 전투 · 플레이어 UI** — [@yeomin-yoon](https://github.com/yeomin-yoon)

- 이동 · 달리기 · 구르기 · 백스텝 조작과 락온 카메라
- Anim Notify State 기반 공격 충돌 판정과 무적 · 패링 타이밍 제어
- 내적으로 마주본 방향을 확인하고 공격 타이밍 · 그로기 상태를 함께 판정하는 패링 치명타
- 화톳불 · 문 상호작용과 체력 · 에스트병 · 소울 · 던전 UI

**보스 AI · 애니메이션 · 게임 상태 · 맵** — [@VaVamVa](https://github.com/VaVamVa)

- Status · Action · Weapon 컴포넌트로 분리한 모듈형 보스 AI
- Data Asset으로 무기별 공격 모션 · 데미지 · 애니메이션 속도 · 소켓을 중앙 관리
- Animation Blueprint State Machine과 Control Rig 기반 보스 모션 제어
- State Enum 중앙 관리와 Level Open/Close, 로딩 UI, 레벨 재활용 재시작

## 협업 방식

- 간트차트로 일정을 관리하고 회의를 짧게 유지해 개인 작업 시간을 확보
- 작업 공간(폴더 · 에셋)을 분리해 Blueprint 에셋의 Git 충돌을 최소화
- 도식화와 스토리보드로 구현 전에 아이디어를 동기화

## 개발 환경

Unreal Engine 5.6 · Blueprint

## 프로젝트 열기

1. Unreal Engine 5.6에서 `BossSoul3.uproject`를 엽니다.
2. 게임 시작 맵은 `Content/Maps/EntryLevel`입니다. 에디터 시작 맵은 별도로 설정되어 있으므로 게임 시작 흐름을 확인할 때는 `EntryLevel`을 엽니다.
3. 에디터에서 플레이합니다.

위 안내는 저장소의 프로젝트 파일과 기본 맵 설정을 기준으로 작성했습니다. 새 환경에서의 실행 여부는 별도로 검증하지 않았습니다.


## 게임 소개

반복된 죽음으로 패턴을 익혀 보스를 공략하는 소울라이크 보스전입니다.
정확한 타이밍의 패링으로 보스를 그로기 상태에 빠뜨려 치명타를 노리고,
화톳불에서 회복하며 다시 도전하는 흐름을 구현했습니다.
높은 난이도의 보스 AI와 정교한 전투 판정으로 도전과 성취감을 목표로 했습니다.

## 주요 구현

**플레이어 캐릭터 · 전투 · 플레이어 UI** — [@yeomin-yoon](https://github.com/yeomin-yoon)

- 이동 · 달리기 · 구르기 · 백스텝 조작과 락온 카메라
- Anim Notify State 기반 공격 충돌 판정과 무적 · 패링 타이밍 제어
- 내적으로 마주본 방향을 확인하고 공격 타이밍 · 그로기 상태를 함께 판정하는 패링 치명타
- 화톳불 · 문 상호작용과 체력 · 에스트병 · 소울 · 던전 UI

**보스 AI · 애니메이션 · 게임 상태 · 맵** — [@VaVamVa](https://github.com/VaVamVa)

- Status · Action · Weapon 컴포넌트로 분리한 모듈형 보스 AI
- Data Asset으로 무기별 공격 모션 · 데미지 · 애니메이션 속도 · 소켓을 중앙 관리
- Animation Blueprint State Machine과 Control Rig 기반 보스 모션 제어
- State Enum 중앙 관리와 Level Open/Close, 로딩 UI, 레벨 재활용 재시작

## 협업 방식

- 간트차트로 일정을 관리하고 회의를 짧게 유지해 개인 작업 시간을 확보
- 작업 공간(폴더 · 에셋)을 분리해 Blueprint 에셋의 Git 충돌을 최소화
- 도식화와 스토리보드로 구현 전에 아이디어를 동기화

## 개발 환경

Unreal Engine 5 · Blueprint
