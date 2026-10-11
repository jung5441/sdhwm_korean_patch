# SUPER DRAGON BALL HEROES WORLD MISSION 한국어 패치툴

PC판과 Nintendo Switch판 **SUPER DRAGON BALL HEROES WORLD MISSION**에 한국어 패치를 적용하기 위한 패치툴입니다.

이 저장소는 PC / Switch 패치툴의 소스와 마스터 빌드 환경을 관리합니다.  
최종 사용자용 패치툴은 GitHub **Releases**에 업로드된 실행 파일을 사용하면 됩니다.

정품 사용을 원칙으로 합니다.

다만 PC판의 경우 Anti cheat를 우회하지 못하여 정품에서는 실행되지 않습니다.

> 원본 게임 데이터는 저장소에 포함하지 않습니다.

---

## 지원 플랫폼

### PC

최종 사용자용 실행 파일:

`SDBH_World_Mission_PC_KR_Patch.exe`

기능:

- 게임 폴더 자동 확인
- 한국어 텍스트 적용
- 한국어 폰트 적용
- 카드/캐릭터명/UI 이미지 한국어화
- WDB 데이터 한국어화
- 30fps 한국어 자막 영상 적용
- 패치 적용 전 원본 CPK 자동 백업
- 패치 업데이트
- 원본 복원

PC 영상은 `AnimeA_5.usm`과 `AnimeA_5_en.usm`을 모두 처리합니다.

### Nintendo Switch

최종 사용자용 실행 파일:

`SDBH_World_Mission_Switch_KR_Patch.exe`

지원 출력:

- Eden
- Atmosphere LayeredFS

Title ID:

`0100E5E00C464000`

원본 Switch 덤프는 직접 수정하지 않으며 별도의 LayeredFS 패키지를 생성합니다.

---

## 사용 방법

### PC

1. Releases에서 PC 패치툴을 받습니다.
2. `SDBH_World_Mission_PC_KR_Patch.exe`를 실행합니다.
3. 게임의 CPK 파일이 있는 폴더를 선택합니다.
4. **한글패치 적용 / 업데이트**를 누릅니다.
5. 작업 완료 후 게임을 실행합니다.

처음 패치할 때 원본 파일은 자동으로 백업됩니다.  
필요할 경우 패치툴의 **원본 복원** 기능을 사용할 수 있습니다.

### Switch

1. Releases에서 Switch 패치툴을 받습니다.
2. `SDBH_World_Mission_Switch_KR_Patch.exe`를 실행합니다.
3. 게임의 `romfs` 또는 `romfs`가 포함된 덤프 폴더를 선택합니다.
4. 출력 폴더를 선택합니다.
5. Eden 또는 Atmosphere를 선택합니다.
6. **Switch 한글패치 만들기**를 실행합니다.
7. 생성된 LayeredFS 패키지를 사용합니다.

---

## 현재 정적 검증 상태

### PC

- 이미지 exact readback: **5,302 / 5,302 PASS**
- 텍스트 검증: **PASS**
- 폰트 검증: **PASS**
- WDB readback: **PASS**
- 30fps VIDEOFIX readback: **PASS**

### Switch

- 이미지 대상: **5,283 / 5,283 PASS**
- 수정 outer resource: **1,592**
- 최종 overlay file: **1,640**
- BT_NAME: **1,644**
- MN_NAME: **1,644**
- WDB: **PASS**
- 30fps VIDEOFIX 포함

정적 검증 성공은 파일 구조 및 readback 검증 결과입니다. 실제 게임 실행 결과는 별도로 확인해야 합니다.

---

## 배포 파일

- PC: `SDBH_World_Mission_PC_KR_Patch.exe`
- Switch: `SDBH_World_Mission_Switch_KR_Patch.exe`

두 배포 EXE는 필요한 패치 자산을 내부에 포함하는 단일 실행 파일입니다.

---

## 주의사항

- 게임 원본 파일을 별도로 보관하는 것을 권장합니다.
- PC판은 패치 적용 전 자동 백업 기능을 사용합니다.
- Switch판은 원본 romfs를 직접 수정하지 않습니다.
- 다른 한글패치/모드와 동시에 사용할 경우 파일 충돌이 발생할 수 있습니다.
- 다른 버전의 게임에서는 정상 동작을 보장하지 않습니다.

---

## Credits

한국어 번역, 이미지 한국어화, 폰트 적용, 패치툴 제작 및 검증 작업에 사용된 공개 도구와 각 프로젝트의 개발자들에게 감사드립니다.

이 프로젝트는 원작 게임 제작사 및 유통사와 관련이 없는 비공식 팬 프로젝트입니다.
