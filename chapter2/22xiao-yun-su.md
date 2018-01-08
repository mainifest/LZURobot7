#肖云宿
---
###项目名称：sinX的积分
---
###项目内容：
![](/picture/xiao-yun-su/01.png)  
该案例用于计算sinx 的积分，输入a、b（角度制）便可得到sinx的积分结果，一下是运行过程及结果：  
首先输入a为0度  
![](/picture/xiao-yun-su/02.png)  
再输入b为45度  
![](/picture/xiao-yun-su/03.png)  
得出结果：  
![](/picture/xiao-yun-su/04.png)  

---
###XML代码
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