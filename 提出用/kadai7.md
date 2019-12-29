# 課題7レポート
原画像を読み込み、白黒濃淡画像に変換した結果を図1、濃淡ヒストグラムを図2に示す。
![原画像](https://github.com/r-takano/lecture_image_processing/blob/master/picture/kadai7/kadai7_1.png)  
図1 変換された白黒濃淡画像
![原画像](https://github.com/r-takano/lecture_image_processing/blob/master/picture/kadai7/kadai7_2.png)  
図2 白黒濃淡画像の濃度ヒストグラム

以下のように、画素のダイナミックレンジを255にする。
ORG = double(ORG);  
mn = min(ORG(:)); % 濃度値の最小値を算出  
mx = max(ORG(:)); % 濃度値の最大値を算出  
ORG = (ORG-mn)/(mx-mn)*255;  

![原画像](https://github.com/r-takano/lecture_image_processing/blob/master/picture/kadai7/kadai7_3.png)  
図3 ダイナミックレンジを拡大した画像

ヒストグラムの表示のためにdoubleに変換したORGをuint8に変換する。
ORG = uint8(ORG);

![原画像](https://github.com/r-takano/lecture_image_processing/blob/master/picture/kadai7/kadai7_4.png)  
図4 濃度ヒストグラム
