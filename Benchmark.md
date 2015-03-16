﻿#summary 分词测试结果
#labels Featured

# 互联网测试 #

  * 对1000句 _BBS_ 中的句子进行人工测试，分词准确度: **96.1%**
  * 对2000句 _菜谱_ 中的句子进行人工测试，分词准确度: **93.7%**


# 人民日报98年一月语料库 #

## CRF 2 Columns ##

process\_chain = prepare, crf2, single\_combine

### 北大语料测试 ###
```
Time: 2975ms
=== SUMMARY:
=== TOTAL INSERTIONS:	782
=== TOTAL DELETIONS:	1553
=== TOTAL SUBSTITUTIONS:	2326
=== TOTAL NCHANGE:	4661
=== TOTAL TRUE WORD COUNT:	104372
=== TOTAL TEST WORD COUNT:	103601
=== TOTAL TRUE WORDS RECALL:	0.963
=== TOTAL TEST WORDS PRECISION:	0.970
=== F MEASURE:	0.966
=== OOV Rate:	1.000
=== OOV Recall Rate:	0.963
=== IV Recall Rate:	--
```

### 微软语料测试 ###
```
Time: 3145ms=== SUMMARY:
=== TOTAL INSERTIONS:	7129
=== TOTAL DELETIONS:	2419
=== TOTAL SUBSTITUTIONS:	8542
=== TOTAL NCHANGE:	18090
=== TOTAL TRUE WORD COUNT:	106873
=== TOTAL TEST WORD COUNT:	111583
=== TOTAL TRUE WORDS RECALL:	0.897
=== TOTAL TEST WORDS PRECISION:	0.860
=== F MEASURE:	0.878
=== OOV Rate:	1.000
=== OOV Recall Rate:	0.897
=== IV Recall Rate:	--
```

## UNIGRAM ##

process\_chain = ascii, unigram, single\_combine

### 北大语料测试 ###
```
Time: 598ms
=== SUMMARY:
=== TOTAL INSERTIONS:	1197
=== TOTAL DELETIONS:	1523
=== TOTAL SUBSTITUTIONS:	2539
=== TOTAL NCHANGE:	5259
=== TOTAL TRUE WORD COUNT:	104372
=== TOTAL TEST WORD COUNT:	104046
=== TOTAL TRUE WORDS RECALL:	0.961
=== TOTAL TEST WORDS PRECISION:	0.964
=== F MEASURE:	0.963
=== OOV Rate:	1.000
=== OOV Recall Rate:	0.961
=== IV Recall Rate:	--
```

### 微软语料测试 ###
```
Time: 783ms
=== SUMMARY:
=== TOTAL INSERTIONS:	9352
=== TOTAL DELETIONS:	1900
=== TOTAL SUBSTITUTIONS:	9779
=== TOTAL NCHANGE:	21031
=== TOTAL TRUE WORD COUNT:	106873
=== TOTAL TEST WORD COUNT:	114325
=== TOTAL TRUE WORDS RECALL:	0.891
=== TOTAL TEST WORDS PRECISION:	0.833
=== F MEASURE:	0.861
=== OOV Rate:	1.000
=== OOV Recall Rate:	0.891
=== IV Recall Rate:	--
```


## CRF 6 Tags + 6 Templates ##

process\_chain = ascii, crf, single\_combine

### 北大语料测试 ###
```
Time: 2138ms
=== SUMMARY:
=== TOTAL INSERTIONS:	648
=== TOTAL DELETIONS:	2190
=== TOTAL SUBSTITUTIONS:	3569
=== TOTAL NCHANGE:	6407
=== TOTAL TRUE WORD COUNT:	104372
=== TOTAL TEST WORD COUNT:	102830
=== TOTAL TRUE WORDS RECALL:	0.945
=== TOTAL TEST WORDS PRECISION:	0.959
=== F MEASURE:	0.952
=== OOV Rate:	1.000
=== OOV Recall Rate:	0.945
=== IV Recall Rate:	--
```

### 微软语料测试 ###
```
Time: 2285ms
=== SUMMARY:
=== TOTAL INSERTIONS:	7174
=== TOTAL DELETIONS:	3119
=== TOTAL SUBSTITUTIONS:	10195
=== TOTAL NCHANGE:	20488
=== TOTAL TRUE WORD COUNT:	106873
=== TOTAL TEST WORD COUNT:	110928
=== TOTAL TRUE WORDS RECALL:	0.875
=== TOTAL TEST WORDS PRECISION:	0.843
=== F MEASURE:	0.859
=== OOV Rate:	1.000
=== OOV Recall Rate:	0.875
=== IV Recall Rate:	--
```