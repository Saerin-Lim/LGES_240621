# LGES_240621

### 실습 준비(새로운 colab 파일에서 실행)

0. 필요 패키지
```py
import zipfile, tarfile
from google.colab import drive # Local PC로 실습하는 경우 실행 x
```
1. 구글 드라이브 연동(Local PC로 실습하는 경우 실행 x)
```py
drive.mount('/content/drive')
%cd /content/drive/MyDrive
```

2. git에서 가져오기
```py
!git clone https://github.com/Saerin-Lim/LGES_240621.git
```

3. cat_dog data 압축풀기
```py
# change directory # Local PC로 실습하는 경우 실행 x
%cd LGES_240621/
```
```py
dog_cat_zip = zipfile.ZipFile('./data/dog_cat.zip')
dog_cat_zip.extractall('./data')
dog_cat_zip.close()
```

4. heros data 압축풀기
```py
heros_zip = zipfile.ZipFile('./data/heros.zip')
heros_zip.extractall('./data')
heros_zip.close()
```

5. torchsummary 설치
```py
!pip install torchsummary
```

6. 해당 tutorial 파일 열기
파일 -> 드라이브에서 찾기 -> 내 드라이브 -> LGES_240621 -> pytorch_tutorial_~~.ipynb
