## 1. ๐ All Eyez on KADIZ๋?

๐ All Eyez on KADIZ๋ 2022๋ ์  4ํ ๊ณต๊ตฐ ํด์ปคํค์ ์ถํํ์ฌ ์ฐ์์์ ์์ํ KADIZ ์นจ๋ฒ ์์ฌ ํญ์ ๋ค์ ๋ํ ๊ฒฝ๋ก ์์ธก ํ๋ก์ ํธ์๋๋ค.
</br>
</br>

## 2. Details of ๐ All Eyez on KADIZ

### 1. ํ๋ก์ ํธ ๊ธฐ๊ฐ
    22. 8. 22. ~ 22. 9. 20.
### 2. Made with
 * [![Jupyter](https://img.shields.io/badge/jupyter-gray?style=for-the-badge&logo=Jupyter)](https://jupyter.org/)
 * [![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)](https://pytorch.org/)
 * [![Folium](https://img.shields.io/badge/Folium-brightgreen?style=for-the-badge&logo=folium&logoColor=white)](http://python-visualization.github.io/folium/)
 * [![Sympy](https://img.shields.io/badge/sympy-%230C55A5.svg?style=for-the-badge&logo=sympy&logoColor=white)](https://www.sympy.org/en/index.html)
 * [![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/docs/index.html)
 ### 3. Dataset 
 * **๐ฅ Problem**</br>
    ํญ์  ๊ฒฝ๋ก ์์ธก์ ํ์์ ์ธ ํญ์  ๊ฒฝ๋ก ๋ฐ์ดํฐ๋ 2๊ธ ๋น๋ฐ๋ก ๋ฐ์ถ ๋ถ๊ฐ
 * **โจ Solution**</br>
    ๋ฐ์ดํฐ๋ฅผ ๋ถ๊ฐํผํ๊ฒ ์์๋ก ์์ฑํด์ผ ํ์ง๋ง ๊ฐ๋ฅํ ์ ๋น์ฑ์๊ฒ ๋ฐ์ดํฐ๋ฅผ ์์ฑํ๊ณ  ์ถ์์ต๋๋ค.</br>
    ๊ทธ๋์ ์ ํฌ๋ ์๋์ ๊ฐ์ด KADIZ ์นจ์๊ด๋ จ ๊ธฐ์ฌ๋ค ์ค ๊ตญ๋ฐฉ๋ถ์ ํฉ๋์ฐธ๋ชจ๋ณธ๋ถ ๋ณด๋์๋ฃ๋ฅผ ๋ฐํ์ผ๋ก KADIZ ์นจ์ ํญ์  ๊ฒฝ๋ก๋ฅผ ์๊ฐํํ ์๋ฃ๋ค์ ์ฐธ๊ณ ํ์ต๋๋ค.</br>
    ์ฌ๋ฌ ์๋ฃ๋ค์ ์กฐ์ฌํ๋ ์ค ์ ํฌ๋ ๋๊ฐ ์ค๊ตญ๊ธฐ์ ๊ฒฝ์ฐ ์ด์ด๋ ๋ถ๊ทผ์์ ๋ถ์ํ์ฌ ๋ํด์์ผ๋ก ํ์ ๊ถค์ ์ ๊ทธ๋ฆฌ๋ฉฐ ์นจ์ํ๋ค๋ ์ฌ์ค์ ๋ฐ๊ฒฌํ์ต๋๋ค.
    <p align="center">
        <img width="419" alt="route" src="https://user-images.githubusercontent.com/42788336/197400385-ed5f8d0a-b746-4e7c-a0b6-54b27f72700e.png">
    </p>
    ๋ฐ๋ผ์ ์๋์ ๊ฐ์ ํ์์ ๋ฐฉ์ ์(ํ์ ๊น์ง ๊ณ ๋ ค)๊ณผ ๊ธฐํธ ์ํ ๋ผ์ด๋ธ๋ฌ๋ฆฌ์ธ Sympy๋ฅผ ์ด์ฉํ์ฌ KADIZ ์นจ์ ํญ์  ๋ฐ์ดํฐ์์ ์์ฑํ์ต๋๋ค. ์ด๋ ํญ์  ๋ฐ์ดํฐ์์ ์๋์ ๊ฒฝ๋๋ก ์ด๋ฃจ์ด์ง ์๊ณ์ด ๋ฐ์ดํฐ์๋๋ค.

```math
Ax^2+By^2+Cx+Dy+Exy+F = 0
```
 ### 4. Preprocessing
    ๊ฒฐ๊ณผ๊ฐ ํน์  feature์ ๊ณผ๋ํ๊ฒ ์ํฅ๋ฐ์ง ์๊ธฐ ์ํด minmaxscaler, standardscaler๋ฅผ ์ฌ์ฉํ์ฌ ์ ์ฒ๋ฆฌ

 ### 5. Modeling
    ์ ํฌ์ ๋ชฉํ๋ ์๊ณ์ด ๋ฐ์ดํฐ์ธ ํญ์  ๋ฐ์ดํฐ์ ์ผ๋ถ๋ฅผ ์๋ ฅ์ผ๋ก ๋ฐ์ ๋ ๊ทธ ํ์ ๊ฒฝ๋ก๋ค์ ์์ธกํ๋ ๊ฒ์ด๊ธฐ ๋๋ฌธ์ ๋ํ์ ์ธ ์๊ณ์ด ๋ถ์ ๋ชจ๋ธ์ธ LSTM์ ์ฌ์ฉํ์ต๋๋ค.
    ์ด๋ loss funtion์ MSE, optimizer๋ Adam์ ์ฌ์ฉํ์ต๋๋ค.

 ### 6. Results
์์ | ํ๋์ | ์ฃผํฉ์
--- | --- | ---
์๋ฏธ | `์ค์  ํญ์  ๊ฒฝ๋ก` | `์์ํ ํญ์  ๊ฒฝ๋ก`

![animation](https://user-images.githubusercontent.com/42788336/197400667-9e9605f1-a56a-4836-b17f-24f73e055317.gif)

 ### 7. References ๐
 [Liu, Yulin, and Mark Hansen. "Predicting aircraft trajectories: a deep generative convolutional recurrent neural networks approach." arXiv preprint arXiv:1812.11670 (2018).](https://arxiv.org/abs/1812.11670)
</br>
</br>

## 3. ํ์ ๊ตฌ์ฑ ๋ฐ ์ญํ 

* [![Seokjin Kim](https://img.shields.io/badge/-%F0%9F%91%A8%F0%9F%8F%BB%E2%80%8D%F0%9F%92%BB%20Seokjin%20Kim-blue)](https://github.com/SukJinKim)</br>
    ํ๋ก์ ํธ ์ด๊ด, ๋ฐ์ดํฐ ์์ฑ ๊ตฌํ, ์ ๋๋ฉ์ด์ ์๊ฐํ ๊ตฌํ ๋ฑ
* [![Yezun Chung](https://img.shields.io/badge/-%F0%9F%91%A8%F0%9F%8F%BB%E2%80%8D%F0%9F%92%BB%20Yezun%20Chung-brightgreen)](https://github.com/Chungyezun)</br>
    ๋ฐ์ดํฐ ์ ์ฒ๋ฆฌ ๋ฐ ๋ชจ๋ธ๋ง ๋ฑ
* [![Dongyeon Kim](https://img.shields.io/badge/-%F0%9F%91%A8%F0%9F%8F%BB%E2%80%8D%F0%9F%92%BB%20Dongyeon%20Kim-orange)](https://github.com/dongyeon22)</br>
    ๋ฐ์ดํฐ ์์ฑ ๊ตฌํ ๋ฑ
