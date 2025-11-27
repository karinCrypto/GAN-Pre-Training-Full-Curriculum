# GAN-Pre-Training-Full-Curriculum
GAN Pre-Training

<p align="center">
  <img src="https://github.com/user-attachments/assets/gan-cover-temp.png" width="80%" />
</p>

<h1 align="center"> GAN Pre-Training Full Curriculum (5-Day Program)</h1>

GAN을 안정적으로 학습하기 위해 필요한 딥러닝 기초부터  
DCGAN, CGAN, Pix2Pix까지 단계적으로 완성하는 5일 구성 커리큘럼입니다.  
모든 Day는 **이론 → 코드 구현 → 실습 → 복습 문제**의 구조로 설계되었습니다.

---

## 📑 Curriculum Overview

- **Day 1.** GAN 학습 전 필수 선행지식 복습  
- **Day 2.** Vanilla GAN 완전 정복  
- **Day 3.** DCGAN & CGAN 완전 정복  
- **Day 4.** Pix2Pix: 조건부 이미지 변환  
- **Day 5.** (선택 사항: CycleGAN, StyleGAN 등 확장 가능)

---

# 🗓️ Day 1  
## 🎯 GAN 학습 전 필수 선행지식 복습

GAN 이해에 필요한 핵심 딥러닝 기반 개념을 정리하는 기초 준비 단계입니다.

### 📚 학습 목표
- GAN 구조 이해에 필요한 딥러닝 기초 복습  
- TensorFlow 기반 코드로 개념 체득  
- 객관식·서술형·코드 실습으로 완전 이해  

### 📌 구성
- 신경망 기본 개념  
- Loss & Optimizer  
- CNN 기초  
- Transposed Convolution  
- 이미지 전처리 & `tf.data`  
- 확률 분포 기초  
- Activation Functions  
- Custom Training Loop (`tf.GradientTape`)  

---

# 🗓️ Day 2  
## 📸 Vanilla GAN 완전 정복

GAN의 기본 구조와 학습 방식 전체를 깊이 있게 분석합니다.

### 📚 학습 목표
- GAN 핵심 원리 이해  
- Generator vs Discriminator 역할 정복  
- TensorFlow & PyTorch Vanilla GAN 구현  
- MNIST 이미지 생성  

### 📌 핵심 개념 정리

#### 1. GAN이란?
- 두 개의 신경망이 경쟁적으로 학습  
- 2014년 Ian Goodfellow 발표  

#### 2. Generator (생성자)
- 입력: 노이즈 벡터  
- 출력: 실제 같은 이미지 생성  
- 목표: 판별자를 속이기  

#### 3. Discriminator (판별자)
- 입력: 이미지  
- 출력: 진짜/가짜 확률  
- 목표: 진짜와 가짜 판별  

#### 4. 실습 구성
- Noise sampling  
- Generator/Discriminator 모델 구성  
- BCE Loss 기반 학습  
- GAN training loop 구현  
- MNIST 이미지 생성  

---

# 🗓️ Day 3  
## 🎨 DCGAN & CGAN 완전 정복

딥러닝 기반 이미지 생성의 핵심 모델 DCGAN/CGAN을 집중 학습하는 단계입니다.

### 📚 학습 목표
- DCGAN의 5대 설계 원칙 완전 이해  
- Transposed Convolution 동작 원리 분석  
- CGAN 조건 결합 방식(Concatenate, Embedding 등) 파악  
- Embedding vs One-Hot 차이 명확히 구분  
- BatchNorm vs InstanceNorm 비교  
- PyTorch 기반 DCGAN·CGAN 구현  

### 📌 주요 내용

#### 1. DCGAN 설계 원칙
- Conv/TransposedConv 기반  
- BatchNorm 사용  
- Pooling 지양  
- FC layer 최소화  
- Activation: G(Tanh), D(LeakyReLU)

#### 2. CGAN 핵심 개념
- 레이블 정보를 G·D에 함께 입력  
- 결합 방식: Concatenate, Embedding, Conditional BatchNorm  

#### 3. 실습
- PyTorch DCGAN 구현  
- CGAN으로 MNIST/패션MNIST 조건부 생성  
- 조건별 이미지 시각화  

---

# 🗓️ Day 4  
## 🖼️ Pix2Pix – 조건부 이미지 변환의 모든 것

Image-to-Image Translation 기반 Pix2Pix 모델을 집중 분석합니다.

### 📚 학습 목표
- Pix2Pix 구조 및 CGAN과의 차이 이해  
- U-Net Generator 구조·skip connection 분석  
- PatchGAN Discriminator 장점 이해  
- Mixed Precision Training 기본 원리  
- TensorFlow Pix2Pix 구현  

### 📌 주요 내용

#### 1. Pix2Pix 구조  
- Input → Output 형태의 Image-to-Image Translation  
- Pair 데이터 기반 학습  

#### 2. U-Net Generator  
- Encoder–Decoder 구조  
- Skip Connection으로 정보 손실 방지  

#### 3. PatchGAN Discriminator  
- 이미지 전체가 아닌 “패치 단위”로 판별  
- 높은 안정성·효율성  

#### 4. Mixed Precision Training  
- FP16 + FP32 혼합 연산  
- GPU 메모리 절약 및 속도 향상  

#### 5. 실습 구성  
- TensorFlow Pix2Pix 구현  
- Edge → Photo 변환  
- Data loader 구성  
- Loss 및 training loop 작성  

---

# Day 5 
CycleGAN, StyleGAN, Diffusion Models 등 확장 과정 구성 가능

---