# 에뮬레이터 보드 버전에 따른 구분
## 버전확인 방법
'/emualtor' 폴더에서 'diag'명령을 사용하면 버전을 확인 할 수 있다.  
cd /emulator  
./diag  

## 두가지 버전
버전은 2.x 버전과 1.x 버전이 있다. 하드웨어에 차이가 있다.  
  2020년 10월 이전에 납품된 모델은 v1.x  이후 모델은 v2.x 이다.  
  
Version 2.x  
      FPGA Bitstream Date     : 20201013   
      FPGA Bitstream Version  : 10021000 (v2.1)  
      
Version 1.x  
      FPGA Bitstream Date     : 20201013   
      FPGA Bitstream Version  : 10011000  (v1.1)       
      

# 저장소 구조
**/rev_v1.x**        *<= 버전 1.x 계측기 프로그램 묶음이 있다. tar.xz로 압축되어 있다.*  
**/rev_v2.x**        *<= 버전 2.x 계측기 프로그램 묶음이 있다. tar.xz로 압축되어 있다.*       
**/doc**             *<= 계측기관련 문서가 올라가 있다.*  
**README.md**        *<= 이문서*  
 
