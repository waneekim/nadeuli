# 행사 지역 지도

기준 자료: **2026-07-01** `vuski/admdongkor`, commit `dd1881663fcabc69b81393604e91ebf3a4202e9a`.

원본: https://github.com/vuski/admdongkor/tree/dd1881663fcabc69b81393604e91ebf3a4202e9a/ver20260701

본 데이터는 통계청 통계지리정보서비스(SGIS, https://sgis.kostat.go.kr)에서 공공누리 제1유형으로 개방한 행정동 경계를 가공한 것이며(가공: vuski/admdongkor, https://github.com/vuski/admdongkor), CC BY 4.0으로 배포됩니다.

- 데이터 이용 조건: https://github.com/vuski/admdongkor/blob/dd1881663fcabc69b81393604e91ebf3a4202e9a/LICENSE-DATA
- CC BY 4.0: https://creativecommons.org/licenses/by/4.0/
- 원자료 SHA256: `c01ef44a0eb00978662ba7a6240ccb1da287fb52abd85104a1758969d391132f`
- 나들이로그의 가공: 읍면동 경계 합치기, 일반시 행정구를 시 단위로 합치기, 좌표 투영·단순화, 고정 이름표 위치 계산.
- 결과: 검색 구역 17개, 시·군·구/시 단위 선택 영역 230개. **17개는 사이트의 여행 지역 분류**이며 현행 광역자치단체 수를 뜻하지 않는다. 광주와 전남은 기존 검색 구역을 유지한다.
- 인천: 제물포구·영종구·서해구·검단구를 포함한 11개 영역. 이전 구명으로 저장된 행사만 명시된 새 경계와 행사 좌표를 대조해 현재 지역 필터로 연결한다.
- 모든 영역은 원자료의 한글 이름과 행정코드에 직접 연결한다. 행사 수·유무·좌표로 지도 이름을 추정하지 않는다.
- 법적 경계 확인용 자료가 아닌 행사 탐색용 단순화 지도다. 원자료의 알려진 정확도 한계는 위 저장소 설명을 따른다.

생성: `python automations/transform/build_korea_map.py`. 로컬 원자료를 쓰려면 `--source <geojson>`; 동일 SHA256만 허용한다.
