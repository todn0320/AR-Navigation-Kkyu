# Polycam + UWB를 활용 Unity + AR Foundation을 사용해 진행

**✅ 1️⃣ Polycam으로 공간 스캔 & 모델링**

•	**Polycam**을 이용해 공간을 **3D 스캔**하고, 이를 **FBX**, **GLTF**, **USDZ** 등의 포맷으로 **Export**해야 해.

•	**iPhone 15 Pro**에서 LiDAR 센서를 사용하면 **정밀한 3D 모델**을 만들 수 있어.

**Export 형식**:

•	**FBX**: Unity에서 가장 많이 사용됨.

•	**GLTF**: 웹용/Unity에서 사용 가능.

•	**USDZ**: iOS/ARKit에 최적화됨.

---

**✅ 2️⃣ Unity에서 3D 모델 불러오기**

•	**Unity 프로젝트**를 만들고, **Polycam**에서 **Export한 3D 모델**을 **Unity**에 임포트.

•	**NavMesh**와 **Collider**를 적용해서, 3D 공간을 **경로 탐색 가능**하게 설정할 수 있어.

**단계별 작업**

1.	**Unity 프로젝트 설정**:

•	Unity Hub에서 새 3D 프로젝트 만들기.

•	AR Foundation과 **ARKit/ARCore** 패키지 설치 (Unity Package Manager).

2.	**Polycam Export 3D 모델 Import**:

•	3D 모델을 Unity에 임포트하고, **Scene**에 배치.

3.	**NavMesh 설정**:

•	**NavMesh**를 생성하여 경로 탐색을 가능하게 설정.

•	**NavMesh Surface** 컴포넌트를 추가하여 공간에 내비게이션을 구현.

4.	**Collider 설정**:

•	공간 내 각 오브젝트에 **Collider**를 추가하여 충돌 처리.

---

**✅ 3️⃣ AR Foundation으로 AR 내비게이션 기능 구현**

•	**AR Foundation**을 사용하면 **ARKit**(iOS)과 **ARCore**(Android)를 동시에 지원할 수 있어.

•	AR 내비게이션 앱에서 **사용자의 위치**를 실시간으로 추적하고, 이를 **3D 공간**에서 경로를 표시하는 방식으로 구현 가능.

**필요한 작업**

1.	**AR Session 설정**:

•	AR Foundation에서 AR을 사용할 수 있도록 **AR Session**을 설정.

•	**AR Camera**를 설정해, 카메라에서 보여주는 실제 공간과 가상 객체를 합성.

2.	**경로 안내 UI 구현**:

•	**UWB** 혹은 **VPS**에서 받은 **실시간 위치 정보**를 기반으로 AR 화면에서 사용자 위치와 목적지까지 경로를 표시.

•	**NavMesh**를 사용해 경로를 탐색하고, 경로에 대한 **PathRenderer**를 만들어 사용자가 쉽게 따라갈 수 있도록 구현.

3.	**UWB 연동**:

•	**UWB Tag**로 실시간 위치 정보를 받아 Unity에서 처리.

•	**Anchor** 위치 정보와 **UWB Tag**의 위치를 바탕으로 **경로 안내**를 AR 화면에 표시.

---

**✅ 4️⃣ Android & iOS 빌드**

•	**Unity**에서 **AR Foundation**을 활용한 AR 내비게이션을 구현한 후, **iOS**와 **Android** 앱으로 빌드하여 모바일 기기에서 실행할 수 있어.

•	빌드 설정에서 각 플랫폼에 맞는 설정을 해야 해 (예: iOS는 ARKit, Android는 ARCore).

**iOS 빌드**

1.	**ARKit 설정**: iOS에 AR 기능을 활성화.

2.	**Xcode로 빌드**: Unity에서 iOS 프로젝트를 빌드하여 Xcode에서 실행.

**Android 빌드**

1.	**ARCore 설정**: Android에 AR 기능을 활성화.

2.	**Android Studio로 빌드**: Unity에서 Android 프로젝트를 빌드하여 Android Studio에서 실행.

---

**✅ 5️⃣ 최적화 및 테스트**

•	**배터리 소모**, **프레임 레이트**, **경로 정확도** 등을 테스트하여 성능을 최적화해야 해.

•	**AR 경험**에서 중요한 점은 **정확한 위치 추적**과 **실시간 반응 속도**이니까 이를 충분히 고려해야 해.

---

**✅ 6️⃣ 앱 기능 추가 (Optional)**

•	**음성 안내**: 경로를 텍스트뿐만 아니라 음성으로도 안내할 수 있어.

•	**UI 디자인**: AR 내비게이션의 경로 외에도, **목적지 설정**, **위치 정보** 등의 UI를 추가하여 직관적으로 사용할 수 있게 할 수 있어.

---

**결론:**

•	**Polycam**으로 3D 모델을 만든 후, **Unity + AR Foundation**을 사용해 AR 내비게이션 앱을 구현.

•	**UWB**를 활용한 **정밀 위치 추적**을 통해 실시간 경로 안내 기능을 추가.

•	**iOS & Android 모두 지원**하는 AR 앱을 완성할 수 있어!