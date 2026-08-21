# 공부할거 — 시스템베릴로그 & UVM 기초 📚

시스템베릴로그(SystemVerilog)와 **UVM(Universal Verification Methodology)** 을 진짜 기초부터 공부하기 위한 자료 모음입니다.
검증(Verification) 입문자를 위해 GitHub 학습 리포지토리와 무료 온라인 튜토리얼을 정리했습니다.

> 정리 기준: **UVM 위주 / 초보자용 / 무료 / 실제로 확인한 링크**

---

## 0. 시작하기 전에 — UVM 공부 순서

UVM은 SystemVerilog의 **객체지향(OOP)** 기능 위에 올라가는 검증 방법론이라, 아래 순서대로 하면 훨씬 수월합니다.

1. **Verilog / SystemVerilog 기본 문법** (신호, always 블록, FSM 등)
2. **SystemVerilog OOP** (class, object, inheritance, virtual, polymorphism)
3. **레이어드 테스트벤치 개념** (driver, monitor, scoreboard)
4. **UVM 핵심 컴포넌트** (uvm_component, agent, sequence, sequencer, driver, monitor, env, test)
5. **UVM 심화** (config_db, factory, TLM, coverage)

---

## 1. 무료 온라인 튜토리얼 (읽기 자료)

가장 처음 개념 잡을 때 보기 좋은 사이트들입니다.

| 사이트 | 설명 |
|---|---|
| [UVM Guide for Beginners (Pedro Araújo)](https://colorlesscube.com/uvm-guide-for-beginners/) | 초보자를 위한 UVM 입문 가이드. 개념을 차근차근 설명해 줌 (강력 추천) |
| [ChipVerify — UVM Tutorial](https://www.chipverify.com/uvm/uvm-tutorial) | UVM 컴포넌트를 하나씩 예제와 함께 설명하는 대표적인 무료 튜토리얼 |
| [Verification Guide — UVM Tutorial](https://verificationguide.com/uvm/uvm-tutorial/) | UVM 계층 구조와 각 컴포넌트를 그림과 코드로 정리 |
| [Verification Academy](https://verificationacademy.com/) | Mentor(Siemens)에서 운영하는 검증 학습 사이트. 무료 강의/포럼 |

---

## 2. GitHub 학습 리포지토리 (기초 → 심화)

직접 코드를 보면서 따라 하기 좋은 학습용 리포지토리입니다.

### 📗 SystemVerilog + UVM 통합 학습
- **[MalykaAwais / Learn_SystemVerilog_and_UVM](https://github.com/MalykaAwais/Learn_SystemVerilog_and_UVM)**
  Verilog 기본부터 SystemVerilog, UVM까지 초보→고급 단계로 정리된 폴더 19개. 디지털 설계 지식이 없는 상태에서 시작한 저자가 만든 자료라 입문자에게 특히 적합.

- **[Abdul-muheet-ghani / UVM-Practice](https://github.com/Abdul-muheet-ghani/UVM-Practice)**
  SystemVerilog OOP부터 시작해서 UVM까지 처음부터 연습한 코드 모음.

- **[harpreetbhatia / sv_practice](https://github.com/harpreetbhatia/sv_practice)**
  SystemVerilog와 UVM 연습 문제/예제.

### 📘 UVM 프로젝트 기반 학습 (작은 예제로 배우기)
- **[XinlueLiu / UVM](https://github.com/XinlueLiu/UVM)** — "Learn UVM by small projects"
  카운터, FIFO, UART 같은 작은 프로젝트로 UVM을 배움. RTL 다이어그램과 UVM 구조 문서 포함. ⭐ 23

- **[amamory-verification / uvm-basics](https://github.com/amamory-verification/uvm-basics)**
  최소 UVM(adder TB)부터 카운터, 곱셈기, NoC 라우터까지 단계별 트레이닝 프로젝트. Questa로 테스트됨. ⭐ 39

- **[irajPatel / UVM-SystemVerilog-Agents-to-Coverage](https://github.com/irajPatel/UVM-SystemVerilog-Agents-to-Coverage)**
  driver, monitor, sequencer → env → scoreboard → coverage까지 UVM 환경을 단계별로 구축하는 가이드.

### 📙 미니멀 UVM 예제 / 템플릿
- **[SeanOBoyle / uvm_example](https://github.com/SeanOBoyle/uvm_example)**
  아주 단순한 DUT + UVM 환경. 확장 가능한 UVM 디렉토리 구조를 보여주는 **템플릿**으로 쓰기 좋음.

- **[chinthacharan / UVM-for-Verification-Basics](https://github.com/chinthacharan/UVM-for-Verification-Basics)**
  검증 기초를 위한 UVM 예제.

- **[VerificationExcellence / UVMReference](https://github.com/VerificationExcellence/UVMReference)**
  UVM 방법론을 사용한 짧은 참고 예제/프로젝트.

### 🐍 (보너스) Python으로 UVM 배우기 — pyuvm
SystemVerilog 문법이 아직 부담되면, 파이썬으로 UVM 개념을 먼저 잡는 것도 좋은 방법입니다.
- **[universal-verification-methodology / learn_uvm_pyuvm](https://github.com/universal-verification-methodology/learn_uvm_pyuvm)**
  Python 기초 → cocotb → UVM 핵심까지 8개 모듈로 구성된 학습 경로. 예제 50개 이상, 설치 자동화 스크립트 포함.

---

## 3. GitHub 토픽 페이지 (더 찾아보고 싶을 때)

최신 리포지토리를 계속 탐색하고 싶을 때 유용합니다.

- [GitHub Topics — `uvm` (SystemVerilog)](https://github.com/topics/uvm?l=systemverilog)
- [GitHub Topics — `uvm-verification`](https://github.com/topics/uvm-verification?l=systemverilog)
- [GitHub Topics — `systemverilog`](https://github.com/topics/systemverilog)

---

## 4. 추천 학습 루트 (요약)

```
1) ChipVerify / Verification Guide 로 SystemVerilog 문벥 훑기
        ↓
2) MalykaAwais/Learn_SystemVerilog_and_UVM 로 SV OOP + 레이어드 TB 연슭
        ↓
3) colorlesscube UVM Guide for Beginners 로 UVM 개념 잡기
        ↓
4) SeanOBoyle/uvm_example 로 UVM 최소 구조 이해 (템플릿)
        ↓
5) XinlueLiu/UVM, amamory-verification/uvm-basics 로 작은 프로젝트 실습
        ↓
6) irajPatel/...Agents-to-Coverage 로 coverage 까지 완성
```

---

*시뮬레이터가 없다면 [EDA Playground](https://www.edaplayground.com/) 에서 브라蚰저로 UVM 코드를 바로 실행해 볼 수 있습니다.*
