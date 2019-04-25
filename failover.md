장애처리
==========

1. 서비스 실행 실패 오류 발생 (Error : 0xc000007b)
   - 분석 내용 : 해당 서비스가 실행 시 종속적인 dll 파일이 64bit경로에 설치되어야 하는게 32bit 경로에 설치되어 해당 오류가 났음.
   - Install Shiled로 프로그램을 설치하는데 64bit인경우 Program Files(x86)에는 32bit용 dll이 설치 되어야하고, Program Files에는 64bit용 dll이 설치되어야 하는데 64bit용 dll이 Program Files(x86)에 덮어 쓴거 같다. 