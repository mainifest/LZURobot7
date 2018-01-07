# 个人案例汇总

---

## 项磊磊

#### 案例名称：猜猜看是几？

这是一个游戏的案例，在平常我们聚会时，我们通常会玩一个游戏：首先，一个人输入一个数字，大家一块去猜，如果数字小了，那么主持人就会提示小了；如果数字大了，那么主持人提示大了。直到我们猜中这个数字。  
这就是这样一个案例，首先展示下它的拼接好的模块图  
![](picture/xiangleilei/01.png)  
下面来运行。首先，我们设定一个数字25  
![](picture/xiangleilei/02.png)  
我们来猜26  
![](picture/xiangleilei/03.png)  
结果呢？多了。  
![](picture/xiangleilei/04.png)  
我们再猜24  
![](picture/xiangleilei/05.png)  
结果少了  
![](picture/xiangleilei/06.png)  
最后，我们输入25  
![](picture/xiangleilei/07.png)  
来看看  
![](picture/xiangleilei/08.png)  
答案正确了。所以下次和朋友聚餐时，可以玩一下试试。

#### JavaScript码
```
var a, b;

b = window.prompt\('请设定数字'\);  
while \(!\(a == b\)\) {  
  a = parseFloat\(window.prompt\('猜猜看'\)\);  
  if \(a &lt; b\) {  
    window.alert\('小'\);  
  } else if \(a &gt; b\) {  
    window.alert\('大'\);  
  }  
}  
window.alert\('Bingo'\);
```
#### XML代码
```
<xml xmlns="http://www.w3.org/1999/xhtml">
  <variables>
    <variable type="" id="SM2_RJEIkiMTOE$kpPcA">a</variable>
    <variable type="" id="5IM(6tU44P%,W!zdb:~$">b</variable>
  </variables>
  <block type="variables_set" id="$)yY@y/rRKpfvWGc!rV@" x="163" y="63">
    <field name="VAR" id="5IM(6tU44P%,W!zdb:~$" variabletype="">b</field>
    <value name="VALUE">
      <block type="text_prompt_ext" id="~eCmk.72eyu!cpu-Sf,O">
        <mutation type="TEXT"></mutation>
        <field name="TYPE">TEXT</field>
        <value name="TEXT">
          <shadow type="text" id="qu3Pt2A(5OH=qf{fVd]Y">
            <field name="TEXT">please set a number of 0 to 100</field>
          </shadow>
        </value>
      </block>
    </value>
    <next>
      <block type="controls_whileUntil" id=";==W__o~(1}TP=uz2PqQ">
        <field name="MODE">UNTIL</field>
        <value name="BOOL">
          <block type="logic_compare" id="@){N_!!-!K(ZL(pWEz$b">
            <field name="OP">EQ</field>
            <value name="A">
              <block type="variables_get" id="`,k/r:`$MN5^Fakj4ty!">
                <field name="VAR" id="SM2_RJEIkiMTOE$kpPcA" variabletype="">a</field>
              </block>
 </value>
            <value name="B">
              <block type="variables_get" id="zkwic?GKfYtA}Bba]BCS">
                <field name="VAR" id="5IM(6tU44P%,W!zdb:~$" variabletype="">b</field>
              </block>
            </value>
          </block>
        </value>
        <statement name="DO">
          <block type="variables_set" id="qfR:wN_.I)JFYPpq`y]/">
            <field name="VAR" id="SM2_RJEIkiMTOE$kpPcA" variabletype="">a</field>
            <value name="VALUE">
              <block type="text_prompt_ext" id="H.5Wkd5IIzzil4Jm$5_p">
                <mutation type="TEXT"></mutation>
                <field name="TYPE">TEXT</field>
                <value name="TEXT">
                  <shadow type="text" id="s}^))-7B82^RrF)`}^H@">
                    <field name="TEXT">take a guess</field>
                  </shadow>
                </value>
              </block>
            </value>
            <next>
              <block type="controls_if" id="5K]lTHT=D9WHtrVp[_LY">
                <mutation elseif="1"></mutation>
                <value name="IF0">
                  <block type="logic_compare" id="ZYoKfLLaqyTjPAgc3s1(">
                    <field name="OP">LT</field>
                    <value name="A">
                      <block type="variables_get" id="q@KTUdRh}.JD25?8f#`B">
                        <field name="VAR" id="SM2_RJEIkiMTOE$kpPcA" variabletype="">a</field>
                      </block>
                    </value>
                    <value name="B">
                      <block type="variables_get" id="XX5vnzEcKFHUFJi`;Quh">
                        <field name="VAR" id="5IM(6tU44P%,W!zdb:~$" variabletype="">b</field>
                      </block>
                    </value>
                  </block>
                </value>
                <statement name="DO0">
                  <block type="text_print" id="d#EG6jTQt^RE4VkM|%`W">
                    <value name="TEXT">
                      <shadow type="text" id="E!XiSmx(sMIj*!pBC.Xz">
                        <field name="TEXT">less</field>
                      </shadow>
                    </value>
                  </block>
                </statement>
                <value name="IF1">
                  <block type="logic_compare" id="Q%`;W.mu,@uxBGrf],+?">
                    <field name="OP">GT</field>
                    <value name="A">
                      <block type="variables_get" id="Yq}Imn6RsWHU,%N,TW!c">
                        <field name="VAR" id="SM2_RJEIkiMTOE$kpPcA" variabletype="">a</field>
                      </block>
                    </value>
                    <value name="B">
                      <block type="variables_get" id="fF|{t`~G@;F;9%ulS+]7">
                        <field name="VAR" id="5IM(6tU44P%,W!zdb:~$" variabletype="">b</field>
                      </block>
                    </value>
                  </block>
                </value>
                <statement name="DO1">
                  <block type="text_print" id="#O$LEi,bljpRU,P!^G_H">
                    <value name="TEXT">
                      <shadow type="text" id="PL9AF-*XiRlGcdU=W(Kp">
                        <field name="TEXT">more</field>
                      </shadow>
                    </value>
                  </block>
                </statement>
              </block>
            </next>
          </block>
        </statement>
        <next>
          <block type="text_print" id="6#hP,WEbP;;Ocv0!;N??">
            <value name="TEXT">
              <shadow type="text" id="^`#h|n^PFddlRTfg`[v|">
                <field name="TEXT">Bingo</field>
              </shadow>
            </value>
          </block>
        </next>
      </block>
    </next>
  </block>
</xml>

```
---
##肖云宿
####案例名称：sinx的积分
![](picture/xiao-yun-su/01.png)  
该案例用于计算sinx 的积分，输入a、b（角度制）便可得到sinx的积分结果，一下是运行过程及结果：  
首先输入a为0度  
![](picture/xiao-yun-su/02.png)   
再输入b为45度  
![](picture/xiao-yun-su/03.png)   
得出结果：  
![](picture/xiao-yun-su/04.png)   
####XML代码
```
<xml xmlns="http://www.w3.org/1999/xhtml">
  <variables>
    <variable type="" id="@JYk)Ht0MhKTTgL9Was$">赋值</variable>
    <variable type="" id="M;7eDV8J4R*79F)~~My*">x</variable>
    <variable type="" id="iS@ye,(;3Md0@{`2Aidw">a</variable>
    <variable type="" id="Rc;Ryn#(}Utt%~rlwmgW">b</variable>
    <variable type="" id=":?#?:pi?aC5bs/JHG(ko">π</variable>
    <variable type="" id="^%WZONX=i.IS}azlU(=_">s</variable>
    <variable type="" id="m{jR-tc]i40GnB`uaxNw">∫sinx</variable>
  </variables>
  <block type="variables_set" id="M#CNnF0V;)i/-7ZBQh^X" x="238" y="188">
    <field name="VAR" id="iS@ye,(;3Md0@{`2Aidw" variabletype="">a</field>
    <value name="VALUE">
      <block type="text_prompt_ext" id="mLZSK;k$0_BoZ0ya2k2C">
        <mutation type="NUMBER"></mutation>
        <field name="TYPE">NUMBER</field>
        <value name="TEXT">
          <shadow type="text" id="fSSJc*-ixJ#/$+(e}23]">
            <field name="TEXT">abc</field>
          </shadow>
        </value>
      </block>
    </value>
    <next>
      <block type="variables_set" id="(@Nt53fBR!x;JXDoYPaA">
        <field name="VAR" id="Rc;Ryn#(}Utt%~rlwmgW" variabletype="">b</field>
        <value name="VALUE">
          <block type="text_prompt_ext" id="]wRC@VhW,r]HMSQ`q1au">
            <mutation type="NUMBER"></mutation>
            <field name="TYPE">NUMBER</field>
            <value name="TEXT">
              <shadow type="text" id="^[$Kj_/zh{}l}`%WugY7">
                <field name="TEXT">abc</field>
              </shadow>
            </value>
          </block>
        </value>
        <next>
          <block type="variables_set" id="_07$tJ7$MY-2nhDt9oJ.">
            <field name="VAR" id="m{jR-tc]i40GnB`uaxNw" variabletype="">∫sinx</field>
            <value name="VALUE">
              <block type="math_arithmetic" id="F_Q:,laKX{@gtF~YsE}D">
                <field name="OP">MINUS</field>
                <value name="A">
                  <shadow type="math_number" id="nYWy^9g{,1r9Ib;^%ebm">
                    <field name="NUM">1</field>
                  </shadow>
                  <block type="math_trig" id="=4l$,a1Hv2x)-|zWvO@e">
                    <field name="OP">COS</field>
                    <value name="NUM">
                      <shadow type="math_number" id="J6d21*RpxrWubab@lCdQ">
                        <field name="NUM">45</field>
                      </shadow>
                      <block type="variables_get" id="2xnxfMF#,QkkPI)fL}2k">
                        <field name="VAR" id="iS@ye,(;3Md0@{`2Aidw" variabletype="">a</field>
                      </block>
                    </value>
                  </block>
                </value>
                <value name="B">
                  <shadow type="math_number" id="j=+X^1SUu_Y*AP),4]^E">
                    <field name="NUM">1</field>
                  </shadow>
                  <block type="math_trig" id="#]T})HW};P%R5Mi/m74!">
                    <field name="OP">COS</field>
                    <value name="NUM">
                      <shadow type="math_number" id="680KbN|VSQvQwemKI+lO">
                        <field name="NUM">45</field>
                      </shadow>
                      <block type="variables_get" id="nb(v.._|w4R|]$S7ulcL">
                        <field name="VAR" id="Rc;Ryn#(}Utt%~rlwmgW" variabletype="">b</field>
                      </block>
                    </value>
                  </block>
                </value>
              </block>
            </value>
            <next>
              <block type="text_print" id="95+RSZxn2fCWabObEX.D">
                <value name="TEXT">
                  <shadow type="text" id="lwq2zSpk.G4P{=~nW26x">
                    <field name="TEXT">abc</field>
                  </shadow>
                  <block type="variables_get" id="pWc8sS~2*mCqKI7^u=QJ">
                    <field name="VAR" id="m{jR-tc]i40GnB`uaxNw" variabletype="">∫sinx</field>
                  </block>
                </value>
              </block>
            </next>
          </block>
        </next>
      </block>
    </next>
  </block>
</xml>

```

---
#吴思睿
####案例名称：
####XML代码
---
#吴铠岚
####案例名称：
####XML代码

---
#武山权
####案例名称：
####XML代码

---
#夏及皓
####案例名称：
####XML代码

---
#吴思清
####案例名称：
####XML代码

---
#张啸岩
####案例名称：
####XML代码


  
























