# RnD_Unreal

## DLC 사용법
1. [Plugin 세팅](#plugin-세팅)  
2. [콘텐츠 오브젝트 생성](#콘텐츠-오브젝트-생성)  
3. [맵(Level) 생성](#맵level-생성)  
4. [프로젝트 런처 세팅](#프로젝트-런처-세팅)  
5. [DLC 테스트](#dlc-테스트)  

---------------

### plugin 세팅  
1. dlc는 plugin 기능이다.  
2. plugin 탭을 오픈  
![image](https://user-images.githubusercontent.com/11674965/162155174-5046048e-7e62-4447-8973-66fe41eb243c.png)  
3. New Plugin 선택  
![image](https://user-images.githubusercontent.com/11674965/162155263-29eb880c-e72c-4582-b9b1-883cd5e8f9ef.png)
4. Plugin 생성  
![image](https://user-images.githubusercontent.com/11674965/162155375-f43f4c1b-cd09-4d30-8118-f4fb4b761d14.png)

### 콘텐츠 오브젝트 생성  
1. 콘텐츠 브라우져에서 new C++ 클릭  
![image](https://user-images.githubusercontent.com/11674965/162155448-75cd87e6-2139-4270-bf6b-556c7cdfcb4a.png)  
2. Actor 생성  
![image](https://user-images.githubusercontent.com/11674965/162156044-88e1c02e-68ae-469b-b936-f974e9354703.png)  

3. c++ 클래스가 플러그인 내부에 배치되도록 하는 작업  
![image](https://user-images.githubusercontent.com/11674965/162156206-f2a0eb4d-e90a-4465-8ab7-56c6664535f2.png)  

4. 플러그인이 제대로 컴파일 되도록 설정되지 않았기 때문에 컴파일 오류가 발생  
![image](https://user-images.githubusercontent.com/11674965/162156233-9abf2908-de3b-41dd-898e-21638f3e32d6.png)  

5. 에디터 오픈 및 모두 무시  
![image](https://user-images.githubusercontent.com/11674965/162156262-26f7be73-31f3-4132-b89f-84bfee5241e4.png)  

6. [Project Name].Build.cs 파일 오픈  
![image](https://user-images.githubusercontent.com/11674965/162156294-efda4225-e34c-474f-a3e7-4e24fae9ac4b.png)  
7. 플러그인 이름을 공용 종속성 모듈 이름에 추가  
![image](https://user-images.githubusercontent.com/11674965/162156355-b1d43f05-a622-4f36-b60e-e4b95ef5a9b8.png)  

8. 프로젝트 빌드  
![image](https://user-images.githubusercontent.com/11674965/162156378-168efcd6-ec55-4d47-82fa-e731ce31b132.png)  

9. 언리얼 프로젝트 닫고 다시 오픈  
C++ 클래스 폴더가 생성되어 있어야함  
![image](https://user-images.githubusercontent.com/11674965/162156459-bd37a800-b105-4ac5-a094-ee04e11d07af.png)  

10. Additional Content에 Bluprints, Maps 폴더 추가  
![image](https://user-images.githubusercontent.com/11674965/162156481-baf4e16f-ce2d-4fb3-9353-fa4c4b9f53ef.png)  

11. C++ 기본 클래스에서 블루프린트 클래스 생성  
![image](https://user-images.githubusercontent.com/11674965/162156511-395a26b5-1ab1-4201-b330-4ade0b9e82ca.png)  

12. 블루프린트 생성  
![image](https://user-images.githubusercontent.com/11674965/162156641-26f1b3df-8a40-4f06-8a8b-a39f05db9350.png)  

13. DefaultSceneRoot에 static mesh 추가  
![image](https://user-images.githubusercontent.com/11674965/162156688-b49de513-4f28-46d2-8e23-28fcb346aa78.png)  

14. 드래그앤 드랍해서 디폴드 대체  
![image](https://user-images.githubusercontent.com/11674965/162156724-a4301fef-b527-4b6e-a6f9-43edd696429b.png)  

15. 뷰옵션 선택  
![image](https://user-images.githubusercontent.com/11674965/162156742-9cccd2f6-cc38-4fc3-a9bb-1551ff04b535.png)  

16. 엔진 콘텐츠 표시 체크  
![image](https://user-images.githubusercontent.com/11674965/162156771-d6c5b33d-4c22-49fe-982a-52da971f925d.png)  

17. Cube 선택  
![image](https://user-images.githubusercontent.com/11674965/162156800-55f64f5a-2963-4e24-8ac5-ff9d97b6e789.png)  

18. Save 및 창 닫기  
19. 엔진콘텐츠 표시 체크 해제  
![image](https://user-images.githubusercontent.com/11674965/162156850-1da31856-3f19-4ba0-90b2-ca6a9e422bd4.png)  

20. 현재 레벨을 다른이름으로 저장  
![image](https://user-images.githubusercontent.com/11674965/162156891-0e900528-df2c-4fb2-8983-799c89ee48e4.png)    
![image](https://user-images.githubusercontent.com/11674965/162156923-c70067b1-5b16-4fe5-ba92-16ff2a61ca13.png)  


### 맵level 생성  
1. Maps 폴더 생성  
![image](https://user-images.githubusercontent.com/11674965/162158261-bce3e47d-601a-4d85-91c3-5cd2ca3e713d.png)  

2. MainMap Save as  
![image](https://user-images.githubusercontent.com/11674965/162158295-9958ee4d-28b3-46c2-a422-c706f84a367d.png)  


3. AdditionalMap 다시 오픈  
![image](https://user-images.githubusercontent.com/11674965/162158327-1ddec9cb-576a-4df7-96ff-fe915cf4ca35.png)  

4. 액터를 레벨에 생성후 저장  
![image](https://user-images.githubusercontent.com/11674965/162158350-1c5cd857-8e8c-44a0-86f7-cfd8e4faa335.png)  
 
5. 프로젝트세팅 오픈  
![image](https://user-images.githubusercontent.com/11674965/162158383-266f6464-c926-4f2d-941d-16f79ef5fb25.png)  
 
6. 에디터 시작맵, 게임 기본맵 세팅  
![image](https://user-images.githubusercontent.com/11674965/162158421-6f85430e-f45d-4e75-aba4-9690cbfdc096.png)  

### 프로젝트 런처 세팅 
1. 1.	프로젝트 런처 열기  
![image](https://user-images.githubusercontent.com/11674965/162158690-d7700478-2733-4b16-a583-cb6f02091903.png)  

2. 2.	커스텀 실행 프로파일 추가  
![image](https://user-images.githubusercontent.com/11674965/162158729-9d7923be-3e57-42d2-a01f-239e1e787dff.png)  

3. 3.	main 아래와같이 설정  
![image](https://user-images.githubusercontent.com/11674965/162158770-079f50b0-acf2-4e73-bf97-6d99c4a0eb66.png)  
![image](https://user-images.githubusercontent.com/11674965/162158790-efb26024-d77f-4613-b777-323259e36c68.png)  
 ![image](https://user-images.githubusercontent.com/11674965/162158802-ff5418f1-8f97-4902-9fc2-825d9c80c10d.png)  


4. 4.	Additional 아래와 같이 설정  
![image](https://user-images.githubusercontent.com/11674965/162158841-fabf8577-bf5c-496d-9ad6-52745105e312.png)  
![image](https://user-images.githubusercontent.com/11674965/162158858-40be43bf-d0d0-4497-8263-b86a3b87c9dc.png)  
![image](https://user-images.githubusercontent.com/11674965/162158868-29abdbb2-02a0-43de-a2c4-ca3013e72429.png)  

5. 5.	순차적으로 빌드  
![image](https://user-images.githubusercontent.com/11674965/162158901-9f73b8cf-5cff-4d89-909c-7358f4fc38ae.png)  

6. 6.	디폴트 경로로 따라왔으면 아래에 pak와 실행파일이 생성됩니다.
Additionalmap Pak :  
`\Plugins\AdditionalMap\Saved\StagedBuilds\WindowsNoEditor\[project1]\Plugins\AdditionalMap\Content\Paks\WindowsNoEditor  `  
Main Map 실행파일 :  
`\Saved\StagedBuilds\WindowsNoEditor  `  

### dlc 테스트  
1.	Additionalmap Pak를 실행파일 pak (아래)경로에 복사  
`\Saved\StagedBuilds\WindowsNoEditor\project1\Content\Paks`  
2.	아래경로의 exe 파일 실행  
`\Saved\StagedBuilds\WindowsNoEditor  `  
3.	~ (1옆의 키) 눌러 콘솔 오픈  
4.	“open AdditionalMap” 입력시 해당 map open됨  

