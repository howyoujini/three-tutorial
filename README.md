# Three.js 6주 커리큘럼

---

## [배경 설명] 
### Three.js란?
Three.js는 사용하기 쉬운, 가볍고, 크로스 브라우저 호환성을 가진 자바스크립트 3D 라이브러리. 
현재 빌드에서는 WebGL 렌더러만 포함되어 있으며, WebGPU(실험적), SVG 및 CSS3D 렌더러도 애드온으로 제공해주고 있다. 

[기본 참고]  
- [Three.js 공식 매뉴얼](https://threejs.org/manual/#ko/fundamentals)  
- [Three.js 디자인베이스 자료](https://designbase.co.kr/threejs-03/)

---

## 1주차: “Hello Cube”  
### 목표: Three.js 앱의 구조 학습

- **Three.js의 3가지 기본 요소**: 장면(Scene), 카메라(Camera), 렌더러(Renderer)
- **기본 학습 내용**:
1. `new THREE.PerspectiveCamera(fieldOfView, aspectRatio, near, far)`의 역할과 속성들
2. `WebGLRenderer`의 `setSize`로 렌더러 사이즈 정하기 (캔버스 사이즈)
3. Scene에 3D 객체 추가 (Mesh > Geometry, Material)
4. Scene을 렌더링하고 애니메이션 설정하기
5. 3D 객체에 애니메이션 주기
6. 계단현상, 드로잉버퍼, HD-DPI 개념 학습
7. `renderer.setSize`를 직접 계산하고 최적화하기
8. 로컬 웹 서버 설정 (localhost:8080) - [Servéz](https://greggman.github.io/servez/) 사용
9. Three.js 클론을 받아 웹 서버 띄우기 후 3D 객체 확인

---

## 2주차: 원시 모델 (Primitives)  
### 목표: 다양한 3D 객체와 재질 학습

- **주요 학습 내용**:
1. 3D 객체(Mesh, Geometry)
2. 재질(Material - MeshBasicMaterial, MeshPhongMaterial)
3. 조명(Lighting - PointLight, AmbientLight)
- [Primitives 예제](https://threejs.org/manual/#ko/primitives) 파일 분석

---

## [🏋️‍♀️OFFLINE] 3주차: 카메라와 씬 그래프  
### 목표: 씬 그래프의 계층적 구조 이해

- **씬 그래프 주요 개념**:
1. **장면(Scene)**: 3D 객체들이 추가되는 최상위 컨테이너
2. **객체(Object3D)**: 모든 3D 객체는 `Object3D`를 상속, 위치, 회전, 크기 속성 포함
3. **부모-자식 관계**: 부모 객체의 변형이 자식에게 자동으로 적용됨
4. **좌표계 변환**: 각 객체는 자신의 좌표계에서 변환
5. **트래버설(순회)**: 씬의 모든 객체를 순회하며 렌더링

[씬 그래프 매뉴얼](https://threejs.org/manual/#ko/scenegraph)

---

## 4주차: 재질(Material) 및 텍스처(Texture), 카메라 컨트롤
### 목표: 카메라 컨트롤과 사용자 상호작용 구현

- **주요 학습 내용**:
1. 재질과 텍스처 다루기
2. `OrbitControls`를 사용한 카메라 이동 및 회전 구현
3. 마우스, 키보드 입력 처리 (Raycasting)
4. 불필요한 렌더링 방지

[카메라 컨트롤 매뉴얼](https://threejs.org/manual/#ko/rendering-on-demand)

---

## [🏋️‍♀️OFFLINE] 5주차: 조명, 그림자, 안개 및 모델 로딩
### 목표: 외부 모델 로딩과 고급 렌더링 기법 학습

- **주요 학습 내용**:
1. 조명(Light)과 그림자(Shadow), 안개(Fog)
2. 3D 모델 파일 형식 (GLTF, OBJ 등) 로딩 방법 (GLTFLoader, OBJLoader)
3. 그림자, 반사, 굴절 등 고급 렌더링 기법 적용
4. 캔버스 투명하게 설정하기 및 디버깅 방법

---

## [🏋️‍♀️OFFLINE] 6주차: 최적화 및 프로젝트 계획
### 목표: Three.js 프로젝트 최적화 학습

- **주요 학습 내용**:
1. 최적화 학습 (프레임 관리, 성능 개선)
2. 다음 작업 계획 논의

**참고**: 오프라인 모임 후 식사하며 다음 1.5개월의 작업 계획을 논의.
