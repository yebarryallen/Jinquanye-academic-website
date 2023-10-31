---
title: ESG 报告词云分行业展示
date: 2023-10-31T06:24:53.291Z
summary: |-
  



  ![](wordcloud_交通运输、仓储和邮政业-g-.png "交通运输、仓储和邮政业")

  ![](wordcloud_信息传输、软件和信息技术服务业-i-.png "信息传输、软件和信息技术服务业")

  ![](wordcloud_农、林、牧、渔业-a-.png "农、林、牧、渔业")

  ![](wordcloud_制造业-c-.png "制造业")



  ![](wordcloud_建筑业-e-.png "建筑业")

  ![](wordcloud_卫生和社会工作-q-.png "卫生和社会工作")

  ![](wordcloud_批发和零售业-f-.png "批发和零售业")

  ![](wordcloud_房地产业-k-.png "房地产业")

  ![](wordcloud_文化、体育和娱乐业-r-.png "文化、体育和娱乐业")

  ![](wordcloud_水利、环境和公共设施管理业-n-.png "水利、环境和公共设施管理业")

  ![](wordcloud_教育-p-.png "教育")

  ![](wordcloud_电力、热力、燃气及水生产和供应业-d-.png "电力、热力、燃气及水生产和供应业")

  ![](wordcloud_科学研究和技术服务业-m-.png "科学研究和技术服务业")

  ![](wordcloud_租赁和商务服务业-l-.png "租赁和商务服务业")

  ![](wordcloud_金融业-j-.png "金融业")

  ![](wordcloud_综合-s-.png "综合")

  ![](wordcloud_采矿业-b-.png "采矿业")
draft: false
featured: false
image:
  filename: wordcloud_采矿业-b-.png
  focal_point: Smart
  preview_only: false
---
```

from wordcloud import WordCloud
import matplotlib.pyplot as plt
font = r'C:\Windows\Fonts\AdobeSongStd-Light.otf'



for index, row in result.iterrows():
    # 选择当前行的内容作为字典
    word_freq_dict = row.to_dict()

    # 创建词云对象
    wordcloud = WordCloud(width=800, height=400, font_path=font, background_color='white').generate_from_frequencies(word_freq_dict)

    # 绘制词云图
    plt.figure(figsize=(10, 5))
    plt.imshow(wordcloud, interpolation='bilinear')
    plt.axis('off')

    # 保存词云图片，文件名以当前行的 index 命名
    plt.savefig(f"wordcloud_{index}.png", bbox_inches='tight')
    plt.close()  # 关闭当前绘图，以便下一次循环绘制新的词云

print("词云生成完成。")
```