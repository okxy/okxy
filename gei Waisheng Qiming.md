[汉语拼音](http://www.cidianwang.com/pinyin)
---
***wang _ _*** 

拼音 A ：ai　an　ao　

拼音 B ：bai　ban　bang　bi　bin　bing　bo　

拼音 C ：cai　can　cao　ce　cen　chan　chang　chao　chen　cheng　chi　chong　chu　chuan　chuang　chun　cong　cui　cun　　

拼音 D ：da　dai　dan　dao　de　di　dong　dou　du　duan　dui　dun

拼音 E ：e　en　er

拼音 F ：fan　fang　fei　fen　feng　fu　

拼音 G ：gai　gang　gao　ge　gen　geng　gong　gou　gu　guan　guang　guo　

拼音 H ：hai　han　hang　hao　he　heng　hong　hou　hua　huai　huan　hui　hun

拼音 J ：ji　jia　jian　jiang　jiao　jie　jin　jing　jiu　ju　juan　jun　

拼音 K ：kai　kang　ke　ken　kuan　kuang　kun　kuo　

拼音 L ：lan　lang　le　lei　li　lin　ling　long　lou　lu　lun　luo　lv　

拼音 M ：mai　man　me　mei　meng　mi　mian　miao　mie　min　ming　mou　mu　

拼音 N ：na　nai　nan　neng　nian　nie　ning　niu　nu　nun　nuo　

拼音 O ：ou

拼音 P ：pai　pan　pei　peng　ping　po　pu　

拼音 Q ：qi　qian　qiang　qiao　qie　qin　qing　qiong　qiu　qu　quan　qun

拼音 R ：ran　rao　ren　rong　ru　rui　run　ruo　

拼音 S ：sai　sen　seng　sha　shai　shan　shang　shao　she　shen　sheng　shi　shu　shuai　shuang　shun　shuo　si　song　su　sui　sun　　

拼音 T ：tai　tang　tao　te　teng　tian　ting　tong　

拼音 W ：wa　wai　wang　wei　wen　wo　wu　

拼音 X ：xi　xia　xian　xiang　xiao　xin　xing　xiu　xu　xuan　xue　xun　

拼音 Y ：ya　yan　yang　yao　ye　yi　ying　yong　you　yu　yuan　yue　yun

拼音 Z ：ze　zeng　zha　zhai　zhan　zhang　zhao　zhe　zhen　zheng　zhi　zhong　zhou　zhu　zhuai　zhun　zhuo　zi　zong　zu　zun


zehua, 

产生单、双字名
---

```
from urllib import request
from itertools import permutations as perm
import re

url = 'https://github.com/okxy/Author-Rank/blob/master/main.md'
try:
    s = request.urlopen(url).read().decode('utf-8')
except:
    pass
ss = re.findall('：.*?<',s)
sss = [i[1:][:-1].split('\u3000') for i in ss]
s3 = [j for i in sss for j in i]
s2 = set(s3)
with open('qiming.txt', 'w', encoding='utf-8') as f:
    n = 0
    for i in perm(s2, 2):
        n += 1
        f.write(''.join(i).capitalize())
        if n%10 == 0:
            f.write('\n\n')
        else:
            f.write(' ')

print('finished.')    
print(n,'names')

```


单名候选 （59292 names）
---
___王___ _ _


