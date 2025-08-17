# polycam + unity

**✅ 1️⃣ Polycam으로 공간 스캔**

•	**LiDAR 모델 (iPhone 15 Pro 등)로 스캔**

•	스캔 후 **3D Mesh 모델 (OBJ / FBX / USDZ 등)로 Export**

---

**✅ 2️⃣ Unity로 3D 모델 가져오기**

•	Polycam에서 **FBX 또는 OBJ 파일로 Export**

•	Unity 프로젝트 안에 **Assets 폴더에 임포트**

•	**AR Foundation / ARKit / ARCore 세팅**

•	3D 공간 맵을 씬 위에 올려서 **가상 공간과 현실 공간 매핑 (Alignment 작업)**

---

**✅ 3️⃣ NavMesh 생성**

•	Unity에서 **3D 모델 바닥면 선택 → Navigation Static 설정**

•	**Navigation Window 열기 → Bake**

•	**NavMesh 생성 완료** → AR 내비게이션 경로 탐색용

---

**✅ 4️⃣ 실시간 위치 연동 (UWB / BLE / VPS)**

•	사용자의 위치를 UWB, BLE, 또는 VPS로 **실시간 좌표 받아오기**

•	받아온 좌표를 Unity 3D 공간의 **User Avatar 또는 Camera 위치로 매핑**

---

**✅ 5️⃣ 경로 탐색 및 AR 표시**

•	목적지 설정 → NavMeshAgent.SetDestination()

•	LineRenderer나 **AR 화살표 Prefab**으로 경로 시각화

•	사용자가 움직일 때마다 실시간 경로 업데이트

•	**AR 공간 위에 경로, 안내 텍스트, 이정표 표시**

---

**✅ 6️⃣ 테스트 및 튜닝**

•	현실 공간과 AR 모델 **위치·스케일 오차 조정**

•	AR 콘텐츠 위치 튜닝 (바닥에 제대로 붙어있는지 등)

•	사용자 인터페이스(UI) 추가 → 목적지 선택 기능 등

---