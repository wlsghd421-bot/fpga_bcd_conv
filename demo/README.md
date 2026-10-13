# BCD→이진수 변환(bcd_conv) 보드 시연 자료 (2026-10-12)

보드: Combo II-DLD-Base (Spartan-7 xc7s75fgga484-1), 입력 ten=DIP_SW1~4, one=DIP_SW5~8, 출력 valid=LED1, bin=LED2~LED8 (LED2가 MSB)

| 파일 | 입력 (ten, one) | 예상 | 확인한 LED 출력 |
|---|---|---|---|
| `bcd_00.jpg` | 0, 0 | valid=1, bin=0000000 | LED1만 점등, 일치 |
| `bcd_12.jpg` | 1, 2 | valid=1, bin=0001100 (12) | LED1, LED5, LED6 점등, 일치 |
| `bcd_99.jpg` | 9, 9 | valid=1, bin=1100011 (99) | LED1, LED2, LED3, LED7, LED8 점등, 일치 |
| `bcd_9_15.jpg` | 9, f(15) | valid=0, bin은 의미 없음(계산값 9×10+15=105) | LED1 소등, bin=1101001(105), 일치 |
| `bcd_conv_demo.MOV` | 입력 변경 영상 | | 아래 "영상" 참고 |

## 영상
영상은 이 폴더에 별도 파일로 추가했다. 원본은 Google Drive에도 있다.

- https://drive.google.com/drive/folders/12eSyuYeHt59GqGelOJes2qq3oCBSRnKJ
