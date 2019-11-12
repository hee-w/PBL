# PBL


MainActivity.java (activity_main.xml, category.xml)
1. ListView 생성
2. ListView의 항목을 누르면 Intent를 통하여 다음 액티비티로 이동

ObjectList.java(toomuch.xml, list.xml)
1. intent에서 받아온 정보를 통해 해당 카테고리의 하위 품목들(ex: brace1, brace2...)을 파이어베이스를 통해
 가져옴
2. 검색 기능 구현( 해당 카테고리에서 품목의 이름 검색 )

ObjectDetail.java(detail.xml, detailist.xml)
1. intent를 통해 받아온 정보(품목의 이름)와 name 속성이 일치하는 품목의 세부사항 출력
  - 이름, 가격, 설명 -> 파이어베이스 실시간 데이터베이스 사용 
  - 이미지 -> 파이어베이스 storage 사용 (MyAppGlideModule.java)
