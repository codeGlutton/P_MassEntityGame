# P_MassEntityGame
매스 엔티티를 적용해보고자 개발한 좀비 퇴치 게임

## Git Commit Comment (깃 커밋 규칙)
```
type: Title

body(Optional)
```
```
Types
+ feat : 기능 추가
+ fix : 오류 수정
+ docs : 문서 추가
```

+ 한글로 작성
+ 무엇을 추가했고 왜 추가했는지 요약

## Project Folder Rules (프로젝트 폴더 규칙)
```
Contents/AC : Project Folder
Contents/AC/SourceArt
Contents/AC/SourceArt/SkletalMesh
Contents/AC/SourceArt/StaticMesh
Contents/AC/SourceArt/Animation
Contents/AC/SourceArt/Texture
Contents/AC/SourceArt/Material
Contents/AC/SourceArt/VFX
Contents/AC/SourceArt/Media
Contents/AC/SourceArt/Sound
Contents/AC/Map
Contents/AC/Data : Curve, DataTable, Parameter Folder
Contents/AC/Blueprint
Contents/AC/Blueprint/AI : Behabior Tree, BlackBoard, EQS
Contents/AC/Blueprint/Anim : Animation BP, AnimMontage

Contents/Test : 각자 테스트 용도 에셋 폴더
Contents/Test/각자 이름 : 각자 이름 폴더 내에서 사용하기
```

## Asset Name Rule (에셋 이름 규칙)
```
Prefix_BaseAssetName_Variant
ex)
MainCharacter's 3rd Skeletion's Texture
== T_MainCharSkeltion_03
```
+ Asset의 Prefix는 단어의 첫 알파벳들을 사용 (ex. Material Instance == MI)
+ Variant가 없는 경우에는 00을 사용하거나 생략 가능
+ 양이 너무 많은 외부 에셋은 냅두기

## Code Type Name Rule (코드 타입에 따른 Prefix 규칙)
```
BP_ : 블루프린트
E : Unreal c++ && BP 열거형 Prefix (※ c++에서는 자동으로 붙음)
F : Unreal c++ && BP 구조체 Prefix (※ c++에서는 자동으로 붙음)
FOn"Verb" : 대리자 Prefix
b : bool Prefix (ex. bIsCompleted, bIsDead)
m : member 변수 Prefix
```

## Code Comment Rule (코드 주석 규칙)
```
/// <summary>
/// 함수 구현 설명
/// </summary>
/// <param name="파라미터명"> 파라미터 값 설명 </param>
/// <returns> 리턴 값 설명 </returns>

/**
 * 함수 구현 설명
 * @param 파라미터명 파라미터 값 설명
 * @return 리턴 값 설명
 */
```
+ Get/Set 함수은 주석 제외
+ 일반 함수는 위의 둘 중 하나의 방식으로 주석 작성
