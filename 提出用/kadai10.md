# 課題10レポート
原画像を読み込み、白黒濃淡画像に変換した結果を図1に示す。
![原画像](https://github.com/r-takano/lecture_image_processing/blob/master/picture/kadai10/kadai10_1.png)  
図1 変換された白黒濃淡画像

プレウィット法でエッジ抽出した画像を図2に示す。  
IMG = edge(ORG,'prewitt');  
![原画像](https://github.com/r-takano/lecture_image_processing/blob/master/picture/kadai10/kadai10_2.png)  
図2 プレウィット法でエッジ抽出した画像

ソベル法でエッジ抽出した画像を図3に示す。  
IMG = edge(ORG,'sobel');  
![原画像](https://github.com/r-takano/lecture_image_processing/blob/master/picture/kadai10/kadai10_3.png)  
図3 ソベル法でエッジ抽出した画像

キャニー法でエッジ抽出した画像を図4に示す。  
IMG = edge(ORG,'canny');  
![原画像](https://github.com/r-takano/lecture_image_processing/blob/master/picture/kadai10/kadai10_4.png)  
図4 キャニー法でエッジ抽出した画像
