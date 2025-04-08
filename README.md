# 🌲 엘리몬의 숲 TEST
외부 에셋은 라이선스 문제로 Git에 포함되지 않으므로 각자 로컬에서 직접 다운로드 및 구성해야 합니다.

---

## ⚙️ 세팅

1. 프로젝트 클론

    ```bash
    git clone https://github.com/Elemons-Forest/Elemons-test.git
    ```

2. `Content/ExternalAssets` 폴더를 직접 생성  
3. 아래 에셋들을 다운로드 후 프로젝트에 추가하고 **정확한 경로**에 배치

    ```
    Content/ExternalAssets/
    ├─ Fantasy_Free
    ├─ MonsterForSurvivalGame
    └─ VRS_LowPolyNatureEssentials
    ```

> ⚠️ `ExternalAssets` 경로가 다르면 레벨에서 에셋이 누락되기 때문에 반드시 동일한 폴더 구조를 유지
> ⚠️ 에셋 추가 시 탐색기 상에서 이동하면 Material 참조가 `null`이 되는 문제 발생
>    => 꼭 Epic Games나 언리얼 에디터 안에서 `프로젝트에 추가`를 눌러서 추가!

---

## 📁 폴더 구조

<pre>
Content
├─ ExternalAssets
│  ├─ Fantasy_Free
│  ├─ MonsterForSurvivalGame
│  └─ VRS_LowPolyNatureEssentials
│
├─ _Main
│  ├─ Animations
│  │  ├─ Characters
│  │  └─ Common
│  ├─ Art
│  │  ├─ Materials
│  │  └─ Meshes
│  ├─ Audio
│  ├─ Blueprints
│  ├─ FX
│  ├─ Levels
│  ├─ Materials
│  └─ UI
│     ├─ Fonts
│     ├─ Textures
│     └─ Widgets
│
├─ __ExternalActors__
│  └─ _Main
│     └─ Levels
│        └─ GrassMap
│
└─ __ExternalObjects__
   └─ _Main
      └─ Levels
</pre>

---

## 💡 팁
### 폴더 이동 했는데 기존 경로에 폴더가 그대로 남아있는 경우
- `Content` 폴더 우클릭 > `Update Redirector References`

---

## 🔐 주의사항
- 커밋하기 전에 유료 에셋이 Git에 올라가지 않았는지 꼭 확인

    ```bash
    git status
    ```
