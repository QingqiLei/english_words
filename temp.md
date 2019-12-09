/*
 * @lc app=leetcode id=1218 lang=java
 *
 * [1218] Longest Arithmetic Subsequence of Given Difference
 *
 * https://leetcode.com/problems/longest-arithmetic-subsequence-of-given-difference/description/
 *
 * algorithms
 * Medium (39.59%)
 * Likes:    156
 * Dislikes: 15
 * Total Accepted:    8.7K
 * Total Submissions: 21.7K
 * Testcase Example:  '[1,2,3,4]\n1'
 *
 * Given an integer array arr and an integer difference, return the length of
 * the longest subsequence in arr which is an arithmetic sequence such that the
 * difference between adjacent elements in the subsequence equals
 * difference.
 * 
 * 
 * Example 1:
 * 
 * 
 * Input: arr = [1,2,3,4], difference = 1
 * Output: 4
 * Explanation: The longest arithmetic subsequence is [1,2,3,4].
 * 
 * Example 2:
 * 
 * 
 * Input: arr = [1,3,5,7], difference = 1
 * Output: 1
 * Explanation: The longest arithmetic subsequence is any single element.
 * 
 * 
 * Example 3:
 * 
 * 
 * Input: arr = [1,5,7,8,5,3,4,2,1], difference = -2
 * Output: 4
 * Explanation: The longest arithmetic subsequence is [7,5,3,1].
 * 
 * 
 * 
 * Constraints:
 * 
 * 
 * 1 <= arr.length <= 10^5
 * -10^4 <= arr[i], difference <= 10^4
 * 
 * 
 */

// @lc code=start
class Solution {
    public int longestSubsequence(int[] arr, int d) {
        Map<Integer, Integer> map = new HashMap<>();
        int res = 0;
        for(int right : arr){
            int left = right - d;
            map.put(right, map.getOrDefault(left, 0)+1);
            res = Math.max(res, map.get(right));
        }
        return res;
    }
    /*
756055468
YuXI290
yang6000780
qingling0606
oyyt12345
568284054
zhongna1225
yxhyForever
503354563
ma19950504
1453602166
15877470645
15523999181 
xyr0303foreveryoung
queen1507608
137336613 
chenchunyu95
wangandhui12138 
1372697161
 WHY10060915
xuhongxuan1017 
17733112580
l65601
wxawqz
15253519600
18435202836 
qingling0606
pantene-ivy
792920098
WJX123496
943581146
gs784741118
q1351779144
756904401
z1663872232
wgx877605852
wgx877605852
13298299418
13703019454
HL978973835
847218077
far0127p
834182537
bilibiliduan
wxid_1vlhun5a192m22
will17862821126
shenfu2333
tiandikuanchang
ch_ris_
15051707685
xsc1307
TVXQ15927537431
gs1710452542
jiajiaaa513
sunnychengsisi
17718299220
Yvonne642674
wxid_cmxa4uckjuf322
16604065362
Lyj_9425
crlm1277095807
zxy13875956408
zyj18829048524
834261326
787316225
 lizeru_
wy1396860
SQiiaa31
fisherorwhy
 guo1367450685
xxl19950124
rilnana
foryoudx
hh752715737
wxid_dmfdgvkxxrqc22
hql67dx
hangy1691233926
detectivecs
muzhe_666
LN__2018
2098160971
xm17306151090
15850751380
aliao1223
dy1885544
wxid_p8stthwgsomv22
1439934049
y942671971
cty19870825
15874260744
HuMin19970917
CX_zcy
14768061433
wuyi-clover
 lalalacccj
 13121050033
214786554 
G19990929
Hu1063740228
w978928705
katie66168 
15213147967
Deer_Lu7
LYP13823273988
lhp89757
luck_ocean
w826310201
shadowy118
xiaobingwowo
cindy759
ves1823
wsh370923
QK-0403520
Einstein_lin678
wd119181799
cmc807149374
a1769099725
13566454547
hzq1151064274
15205020896
ATSUYUKO710
bingdmt2018
13998282436
871612499
18007816664
15574778708
605320753
756055468
1875180309
503354563
ma19950504
321889843
137336613
wxawqz
15253519600
13739293896
pantene-ivy
zxztwl 
lxy1042467079
msj0123456789
15549459932
DiyaLi0501 
G15762415707
Eternal_013
bilibiliduan
yen0295
OFjyz112020
huyuan970618
dj0214lala
zj846238970
will17862821126
微信gs1710452542求拉
Yvonne642674
he8525215179
Lyj_9425
fy1522651
anlan1298
13998282436
yixinzhou001
zqy464603034
LoveYI_KE
ab1430671690

wojiaozhangtiancai
Ket412
Ty_cyclebunny
lulaodashigebaobao
jooreyzr 
545761201 
wxid_z489eamdfavj22
zalahahaxz
CJY-970430712
ves1823
yxf990528
871612499
Ket412
recant
jiji22_
Zb5203-Zh

+++++++Mint_LL
// xxp0613
// 371493739
// nikihui
// xujiahui2985









    */
}

// @lc code=end

