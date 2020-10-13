# 저장소 구조
**/rev_v1.x**        *<= 버전 1.x 계측기 프로그램 묶음이 있다. tar.xz로 압축되어 있다.*  
**/rev_v2.x**        *<= 버전 2.x 계측기 프로그램 묶음이 있다. tar.xz로 압축되어 있다.*       
**/doc**             *<= 계측기관련 문서폴더.*  
**README.md**        *<= 이문서*  
**revision.md**      *<= 펌웨서 리비전 정보*
 
# 에뮬레이터 보드 버전에 따른 구분
#### 버전확인 방법
'/emualtor' 폴더에서 'diag'명령을 사용하면 버전을 확인 할 수 있다.  
cd /emulator  
./diag  

#### 두가지 버전
버전은 2.x 버전과 1.x 버전이 있다. 하드웨어에 차이가 있다.  
  2020년 10월 이전에 납품된 모델은 v1.x  이후 모델은 v2.x 이다.  
  
Version 2.x  
      FPGA Bitstream Date     : 20201013   
      FPGA Bitstream Version  : 10021000 (v2.1)  
      
Version 1.x  
      FPGA Bitstream Date     : 20201013   
      FPGA Bitstream Version  : 10011000  (v1.1)       
      
# 계측기 업데이트 방법  
1. revision.md로 최신버전을 확인 한다.  
2. /rev_v1.x 또는 /rev_v2.x 폴더에서 원하는 버전을 다운 받는다. ex) rev_2v1.tar.xz   
3. 파일질라같은 어플을 이용하여 계측기에 '/최상위폴더'에 복사 한다. 다음 명령을 쳐서 파일이 복사된것을 확인한다.  
cd /  
ls /rev_2v1.tar.xz  
4. 현재 계측기 폴더를 백업한다.  
cp -rf /emulator /emulator_bak  
5. 압축을 풀더서 업데이트를 진행한다.  
cd /  
tar -xvf ./rev_2v1.tar.xz  
6. 완료되면 다음 명령을 친다.  
sync  
7. 계측기 전원을 껏다가 켠다.  
8. 버전을 확인해서 업데이트가 됐는지 확인한다.  

### 업데이트 명령어 요약
계측기 최상위 폴더에 'rev_2v1.tar.xz'파일이 복사됐다고 가정하고. 
cd /  
ls /rev_2v1.tar.xz  
cp -rf /emulator /emulator_bak   
tar -xvf ./rev_2v1.tar.xz  
sync  
