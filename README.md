## 1. 👀 All Eyez on KADIZ란?

👀 All Eyez on KADIZ란 2022년 제 4회 공군 해커톤에 출품하여 우수상을 수상한 KADIZ 침범 의심 항적들에 대한 경로 예측 프로젝트입니다.
</br>
</br>

## 2. Details of 👀 All Eyez on KADIZ

### 1. 프로젝트 기간
    22. 8. 22. ~ 22. 9. 20.
### 2. Made with
 * [![Jupyter](https://img.shields.io/badge/jupyter-gray?style=for-the-badge&logo=Jupyter)](https://jupyter.org/)
 * [![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)](https://pytorch.org/)
 * [![Folium](https://img.shields.io/badge/Folium-brightgreen?style=for-the-badge&logo=folium&logoColor=white)](http://python-visualization.github.io/folium/)
 * [![Sympy](https://img.shields.io/badge/sympy-%230C55A5.svg?style=for-the-badge&logo=sympy&logoColor=white)](https://www.sympy.org/en/index.html)
 * [![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/docs/index.html)
 ### 3. Dataset 
 * **💥 Problem**</br>
    항적 경로 예측에 필수적인 항적 경로 데이터는 2급 비밀로 반출 불가
 * **✨ Solution**</br>
    데이터를 불가피하게 임의로 생성해야 했지만 가능한 신빙성있게 데이터를 생성하고 싶었습니다.</br>
    그래서 저희는 아래와 같이 KADIZ 침입관련 기사들 중 국방부와 합동참모본부 보도자료를 바탕으로 KADIZ 침입 항적 경로를 시각화한 자료들을 참고했습니다.</br>
    여러 자료들을 조사하던 중 저희는 대개 중국기의 경우 이어도 부근에서 북상하여 동해상으로 타원 궤적을 그리며 침입한다는 사실을 발견했습니다.
    <p align="center">
        <img width="419" alt="route" src="https://user-images.githubusercontent.com/42788336/197400385-ed5f8d0a-b746-4e7c-a0b6-54b27f72700e.png">
    </p>
    따라서 아래와 같은 타원의 방정식(회전까지 고려)과 기호 수학 라이브러리인 Sympy를 이용하여 KADIZ 침입 항적 데이터셋을 생성했습니다. 이때 항적 데이터셋은 위도와 경도로 이루어진 시계열 데이터입니다.
```math
Ax^2+By^2+Cx+Dy+Exy+F = 0
```
 ### 4. Preprocessing
    결과가 특정 feature에 과도하게 영향받지 않기 위해 minmaxscaler, standardscaler를 사용하여 전처리

 ### 5. Modeling
    저희의 목표는 시계열 데이터인 항적 데이터의 일부를 입력으로 받을 때 그 후의 경로들을 예측하는 것이기 때문에 대표적인 시계열 분석 모델인 LSTM을 사용했습니다.
    이때 loss funtion은 MSE, optimizer는 Adam을 사용했습니다.

 ### 6. Results
 <span style="color:blue; font-weight:bold;">파란색: 실제 항적 경로</span>&emsp;&emsp;<span style="color:orange; font-weight:bold;">주황색: 예측한 항적 경로</span>
 ![animation](https://user-images.githubusercontent.com/42788336/197400667-9e9605f1-a56a-4836-b17f-24f73e055317.gif)

 ### 7. References 📚
 [Liu, Yulin, and Mark Hansen. "Predicting aircraft trajectories: a deep generative convolutional recurrent neural networks approach." arXiv preprint arXiv:1812.11670 (2018).](https://arxiv.org/abs/1812.11670)
</br>
</br>

## 3. 팀원 구성 및 역할

* [![Seokjin Kim](https://img.shields.io/badge/-%F0%9F%91%A8%F0%9F%8F%BB%E2%80%8D%F0%9F%92%BB%20Seokjin%20Kim-blue)](https://github.com/SukJinKim)</br>
    프로젝트 총괄, 데이터 생성 구현, 애니메이션 시각화 구현 등
* [![Yezun Chung](https://img.shields.io/badge/-%F0%9F%91%A8%F0%9F%8F%BB%E2%80%8D%F0%9F%92%BB%20Yezun%20Chung-brightgreen)](https://github.com/Chungyezun)</br>
    데이터 전처리 및 모델링 등
* [![Dongyeon Kim](https://img.shields.io/badge/-%F0%9F%91%A8%F0%9F%8F%BB%E2%80%8D%F0%9F%92%BB%20Dongyeon%20Kim-orange)](https://github.com/dongyeon22)</br>
    데이터 생성 구현 등
