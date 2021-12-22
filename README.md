# kobert_ipc_classification
IPC code classification using KoBERT with patent data

## target
> 
> - 특허문서의 IPC 코드 중 subclass까지
> 
> ![image](https://github.com/jungsungmoon/kobert_ipc_classification/blob/main/pic/1.png)


## input
> 
> - 산업분류코드
>
> ![image](https://github.com/jungsungmoon/kobert_ipc_classification/blob/main/pic/2.png)
>
> - 산업분류코드 + 특허문서의 title, claim, abstract
>
> ![image](https://github.com/jungsungmoon/kobert_ipc_classification/blob/main/pic/3.png)

## target to label
> - IPC 코드를 label로 변환
> 
> ![image](https://github.com/jungsungmoon/kobert_ipc_classification/blob/main/pic/4.png)

## input tokenizing
> - KoBERT 토크나이저 이용
>
> ![image](https://github.com/jungsungmoon/kobert_ipc_classification/blob/main/pic/5.png)

## result
> - 세세분류코드까지 이용해서 IPC를 분류하는 모델이 가장 성능이 좋음
> - 세세분류코드는 해당 데이터로 예측이 불가능
> - 예측가능한 산업분류코드인 중분류코드까지 사용했을 때 약간의 성능 향상
> ![image](https://github.com/jungsungmoon/kobert_ipc_classification/blob/main/pic/6.png)
