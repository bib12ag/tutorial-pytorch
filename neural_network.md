## 🔸 Neural Network 구성하기
- `nn.Module` : 상속받아 클래스 작성
- `super().__init__()` : 부모 클래스 초기화를 통해 속성 사용 가능
- `super(SUBCLASS, self)` : 기능적 차이는 없지만, 현재 클래스를 명확하게 표시

-  `forward()` : `nn.Module`을 상속받은 클래스의 입력 데이터에 대한 연산 구현 메소드, 직접 호출 X
<br>

## 🔹 torch.nn 
신경망을 구성하는데 필요한 모든 모듈 제공

### *Container*
- `Module`
  - 모든 신경망 모듈의 base class
  - 이 클래스를 상속하여 모델 구축

### *Convolution Layers*
- `Conv1d, Conv2d, Conv3d`