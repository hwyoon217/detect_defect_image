# detect_defect_image  
사과 결함 이미지 판별 — OpenCV 기반 이미지 처리 프로젝트

<br>

## 목차
- [소개](#소개)  
- [프로젝트 목표](#프로젝트-목표)  
- [사용 기술](#사용-기술)  
- [데이터 & 처리 방식](#데이터--처리-방식)  
- [실행 방법](#실행-방법)  

<br>

## 소개  
이 프로젝트는 사과 이미지에서 멍이나 흠집 같은 결함을 감지하는 목적으로 개발되었습니다.  
이미지 증강 + 마스크 생성 + Adaptive Threshold 등의 이미지 처리 기법으로 결함을 탐지합니다.  

<br>

## 프로젝트 목표  
- 다양한 사과 이미지에 대해 결함 여부 판별  
- 이미지 증강을 통해 데이터 다양성 확보  
- 마스크 및 Adaptive Threshold 기법을 활용하여 결함 영역 검출  
- 결과에 대한 간단한 성능 평가  

<br>

## 사용 기술  
- Python  
- OpenCV: 이미지 처리, 마스크 생성, Threshold 적용  
- NumPy: 이미지 배열 연산  
- scikit-learn: ROC AUC 등 결함 판별 성능 평가

<br>

## 데이터 & 처리 방식  
- 입력 이미지: 사과 사진 (테스트용 이미지 폴더에 저장)  
- 처리 흐름:  
  1. 이미지 증강 → 다양한 조합의 이미지 생성  
  2. 마스크 생성 및 Adaptive Threshold 적용 → 결함 영역 검출  
  3. 모델에 대한 판별 성능 평가  
  4. 여러 이미지에 대해 일괄 테스트

<br>

## 실행 방법  
- 필요한 라이브러리 설치
```bash
pip install opencv-python numpy scikit-learn
```

- 주피터 노트북에서 실행
```bash
jupyter notebook detect_defect_img.ipynb
```
