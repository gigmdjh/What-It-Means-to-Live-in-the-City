# 무기 PNG 에셋

이 폴더에 무기 PNG를 넣고 저장소 루트에서 아래 명령을 실행하세요.

```bash
python -m pip install Pillow
python tools/convert_weapons.py
```

- 파일명은 게임 코드의 무기 외형 키와 맞춥니다. 예: `tiantui.png`
- 투명 배경을 지원합니다.
- 이미지는 실행 전에 32×32로 최근접 보간 변환됩니다.
- 변환 결과는 루트의 `weapon-pixels.js`에 정적 RGBA 픽셀 데이터로 저장됩니다.
- 게임 실행 중 PNG 파일을 불러오지 않습니다. PNG를 추가하거나 바꾼 뒤에는 변환 도구를 다시 실행하고 `weapon-pixels.js`를 커밋해야 합니다.
