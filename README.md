# 웹 사이트 captcha 무력화를 위한 OCR 성능비교
* * *
* google , kakao 의 open api 성능 비교 (완료 2020-09-29)
    1. 데이터 수집(크롤링) -257개 
    2. 데이터 수집시 수기입력하여 통과할경우 입력번호를 img_name으로 레이블링 진행   
    3. kakao ocr api 발급 받아 정확도 확인 -> 28.0% (52/257)
    4. google vision api 발급 받아 정확도 확인 -> 53.6%
    5. 결과 값만을 뱉어낸 경우 구글 vision의 성능이 더뛰어나다
    6. 숫자 0 -> 알파벳 O , 숫자 1을 -> 알파벳 L or I , 숫자 7 -> 알파벳 X 로 인식하는 경우가 많아     
       결과값에 대한 간단한 추가 처리를 해주면 더욱 성능 향상이 기대 된다.
    
* * *
* 딥러닝 기술을 이용한 정확도 개선 - (데이터 수집 및 모델 구축 중)
    1. 데이터가 2000개 이상 모인다면 CNN기반의 자체 모델을 만들어 성능 평가를 진행예정
    2. 데이터 수집과정에서 6개의 숫자를 각각 나누는 경우와 6개 연속의 전체 이미지에 대한 모델 구축 및 평가 진행예정



* * *
<img src="/img/993244_2020_09_28_15_31_45.png" width="10%" height="5%" title="px(픽셀) 크기 설정" alt="RubberDuck"></img>   
<img src="/img/012445_2020_09_28_16_08_54.png" width="10%" height="5%" title="px(픽셀) 크기 설정" alt="RubberDuck"></img>   
<img src="/img/027221_2020_09_28_15_43_30.png" width="10%" height="5%" title="px(픽셀) 크기 설정" alt="RubberDuck"></img>   
<img src="/img/042852_2020_09_28_15_30_01.png" width="10%" height="5%" title="px(픽셀) 크기 설정" alt="RubberDuck"></img>   
<img src="/img/128811_2020_09_27_17_59_48.png" width="10%" height="5%" title="px(픽셀) 크기 설정" alt="RubberDuck"></img>   
<img src="/img/129737_2020_09_28_16_15_52.png" width="10%" height="5%" title="px(픽셀) 크기 설정" alt="RubberDuck"></img>   
<img src="/img/130251_2020_09_27_18_00_08.png" width="10%" height="5%" title="px(픽셀) 크기 설정" alt="RubberDuck"></img>   

 <img_폴더의 captcha 예시>
