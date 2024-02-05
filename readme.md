## �������ѧϰ�Ĺ������

### ��һ�£���װ�Լ���������

#### 1.Pycharm��װ

```
����: https://www.jetbrains.com/pycharm/
```

#### 2.Anaconda��װ������

```
������https://www.anaconda.com/download#downloads

���û��������������Լ��İ�װ·���������ü��ɣ�
D:\software\anaconda\install
D:\software\anaconda\install\Scripts
D:\software\anaconda\install\Library\bin
D:\software\anaconda\install\Library\mingw-w64\bin
```

#### 3.Tensorflow��װ

```
������https://tensorflow.google.cn/?hl=zh-cn

�������ѧϰ����������Ϊtf2��ָ��python�汾Ϊ3.11:
conda create --name tf2 python=3.11

Anaconda����tf2����:
conda activate tf2

Anaconda�˳������:
conda deactivate


��װTensorflow��ָ���汾Ϊ2.15��ʹ�ö���Դ���м���
pip install tensorflow==2.15.0 -i https://pypi.douban.com/simple/

��װscikit-learn��ʹ�ö���Դ���м���
pip install scikit-learn -i https://pypi.douban.com/simple/
```



### �ڶ��£����뽲�������е���

#### 0.���ݼ�˵��

```
��˹������ѧ������ݼ�������
https://engineering.case.edu/bearingdatacenter/download-data-file

���ݼ�˵��(�����ڹ������ݼ�˵��)��
�ռ���������С����������˺ͷ��ȶ�ȱ�ݵ����ݡ����������ʵ����12000������/���48000������/����ٶȲɼ����ݡ����з�������������12000������/����ٶȲɼ���

�����ļ�ΪMatlab��ʽ��ÿ���ļ��������Ⱥ��������������Լ����ת�١����������ļ����������е��������ʾ:

���ݼ�������
(1)������������
(2)12k��������й�������
(3)48k��������й�������
(4)�������й�������

ʵ�����ݼ���ʹ��12k��������й������ݣ��������ݼ�Ԥ������ʵ������Ԥ����һ�¡�
```



#### 1.���ھ��������Ĺ�����ϣ�1DCNN��2DCNN��

```
�ļ���˵����
data�����ݼ����·��
save_picture/1DCNN:���1DCNN��ͼƬ
save_picture/2DCNN:���2DCNN��ͼƬ

model/1DCNN.h5: �����1DCNNģ���ļ�
model/2DCNN.h5: �����2DCNNģ���ļ�

code/1DCNN.py: 1DCNN���������ļ�
code/2DCNN.py: 2DCNN���������ļ�
code/preprocessing.py: ����Ԥ�����ļ�
```

#### 2.���ھ����ѭ��������Ĺ������(1DCNN-LSTM��1DCNN-GRU��2DCNN-LSTM��2DCNN-GRU)

```
�ļ���˵����
data�����ݼ����·��

save_picture/1DCNN_GRU:���1DCNN_GRU��ͼƬ
save_picture/1DCNN_LSTM:���1DCNN_LSTM��ͼƬ
save_picture/2DCNN_GRU:���2DCNN_GRU��ͼƬ
save_picture/2DCNN_LSTM:���2DCNN_LSTM��ͼƬ


model/1DCNN_GRU.h5: �����1DCNN_GRUģ���ļ�
model/1DCNN_LSTM.h5: �����1DCNN_LSTMģ���ļ�
model/2DCNN_GRU.h5: �����2DCNN_GRUģ���ļ�
model/2DCNN_LSTM.h5: �����2DCNN_LSTMģ���ļ�

code/1DCNN_GRU.py: 1DCNN_GRU���������ļ�
code/1DCNN_LSTM.py: 1DCNN_LSTM���������ļ�
code/2DCNN_GRU.py: 2DCNN_GRU���������ļ�
code/2DCNN_LSTM.py: 2DCNN_LSTM���������ļ�
code/preprocessing.py: ����Ԥ�����ļ�
```

#### 3.���ھ��������С���任�Ĺ������(1DCNN-CWT��2DCNN-CWT)

```
1.����ʱע���������pywt��İ�װ��Ӧʹ�ã�
pip install PyWavelets -i https://pypi.douban.com/simple/

2.�����ڴ���cwt_picture-train-valid-test�ļ��У�������sign_cwt�ļ�����train��valid��test�ļ���������Ӧ������С���任��ͼƬ��������1DCNN_CWT/2DCNN_CWT���з���ʵ��  

�ļ���˵����
data�����ݼ����·��

cwt_picture/train: ���ѵ����������С��ͼƬ
cwt_picture/test: ��Ų��Լ�������С��ͼƬ
cwt_picture/valid: �����֤��������С��ͼƬ

save_picture/1DCNN_CWT:���1DCNN_CWT��ͼƬ
save_picture/2DCNN_CWT:���2DCNN_CWT��ͼƬ

model/1DCNN_CWT.h5: �����1DCNN_CWTģ���ļ�
model/2DCNN_CWT.h5: �����2DCNN_CWTģ���ļ�

code/1DCNN_CWT.py: 1DCNN_CWT���������ļ�
code/2DCNN_CWT.py: 2DCNN_CWT���������ļ�
code/gen_cwt_pic.py: ��������С���任ͼƬ���������ļ�
code/read_picture.py: ��ȡ����С��ͼƬ���������ļ�
code/preprocessing.py: ����Ԥ�����ļ�
```

#### 4.���������ںϵĹ�����ϣ�SIGN-FFT��

```
�ļ���˵����
data�����ݼ����·��

save_picture/1DCNN_SIGN_FFT:���1DCNN_SIGN_FFT��ͼƬ

model/1DCNN_SIGN_FFT.h5: �����1DCNN_SIGN_FFTģ���ļ�

code/1DCNN_SIGN_FFT.py: 1DCNN_SIGN_FFT���������ļ�
code/preprocessing.py: ����Ԥ�����ļ�
```

#### 5.���ڿ��뷽���Ĺ�����ϣ�1DCNN��2DCNN-DRSN��1DCNN-SVD��

```
�ļ���˵����
data�����ݼ����·��

save_picture/1DCNN:���1DCNN��ͼƬ
save_picture/1DCNN_SVD:���1DCNN_SVD��ͼƬ
save_picture/2DCNN_DRSN:���2DCNN_DRSN��ͼƬ

model/1DCNN.h5: �����1DCNNģ���ļ�
model/1DCNN_SVD.h5: �����1DCNN_SVDģ���ļ�
model/2DCNN_DRSN.h5: �����2DCNN_DRSNģ���ļ�

code/1DCNN.py: 1DCNN���������ļ�
code/1DCNN_SVD.py: 1DCNN_SVD���������ļ�
code/2DCNN_DRSN.py: 2DCNN_DRSN���������ļ�
code/plot_svd.py: ��Ϊ������ҪͼƬ���Ϳ��ӻ�һ��������������������
code/preprocessing.py: ����Ԥ�����ļ�
```

#### 6.����Ǩ��ѧϰ�Ĺ�����ϣ�ģ�ͣ�

```
�ļ���˵����
data�����ݼ����·��

save_picture/1DCNN_Transfer:���1DCNN_TransferǨ�Ƶ�ͼƬ

model/1DCNN_Transfer.h5: �����1DCNN_Transferģ���ļ�

code/1DCNN_Transfer.py: 1DCNN_Transfer���������ļ�
code/preprocessing.py: ����Ԥ�����ļ�
```

#### 7.����ͨ��ģ�ʹ���Ĺ�����ϣ�GRU��Inception��LSTM��RandomForest��SVM��

```
�ļ���˵����
data�����ݼ����·��

save_picture/GRU:���GRU��ͼƬ
save_picture/Inception:���Inception��ͼƬ
save_picture/LSTM:���LSTM��ͼƬ

model/GRU.h5: �����GRUģ���ļ�
model/Inception.h5: �����Inceptionģ���ļ�
model/LSTM.h5: �����LSTMģ���ļ�

code/preprocessing.py: ����Ԥ�����ļ�
code/GRU.py: GRU���������ļ�
code/Inception.py: Inception���������ļ�
code/LSTM.py: LSTM���������ļ�
code/RandomForest.py: RandomForest���������ļ�
code/SVM.py: SVM���������ļ�
```











