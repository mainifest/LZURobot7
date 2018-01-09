#张啸岩
---
###案例名称：计算任意小于200的数累加到200的结果
---
###案例内容：
1.案例说明  
具体操作过程为定义a为一个小于200的数字，sum为零，赋值给a后，进入循环语句，则sum等于该轮中的a值和上轮中的sum值，a每轮循环中加一，当a大于200时循环结束，得到结果。
2.界面和模块截图  
![](/picture/zhang-xiao-yan/01.png)  
3.运行测试
![](/picture/zhang-xiao-yan/02.png)  
![](/picture/zhang-xiao-yan/03.png)  

---
###XML代码    
```
<xml xmlns="http://www.w3.org/1999/xhtml">
  <variables>
    <variable id="664nQAmBX{%+.a4:(Uk}" type="">a</variable>
    <variable id="?YYJ/c@uyS!N3P+n3Oeq" type="">sum</variable>
  </variables>
  <block id="y7v+M0ECE^h5XFdYM7kQ" type="variables_set" x="138" y="38">
    <field id="664nQAmBX{%+.a4:(Uk}" name="VAR" variableType="">a</field>
    <value name="VALUE">
      <block id="aZ,B{UTu?S)4)mx(pDR=" type="text_prompt_ext">
        <mutation type="NUMBER"></mutation>
        <field name="TYPE">NUMBER</field>
        <value name="TEXT">
          <shadow id="y22pIEa}Uuu)vl?9h@a9" type="text">
            <field name="TEXT">a</field>
          </shadow>
        </value>
      </block>
    </value>
    <next>
      <block id="stOb*D#h1i-$``ia!MB_" type="variables_set">
        <field id="?YYJ/c@uyS!N3P+n3Oeq" name="VAR" variableType="">sum</field>
        <value name="VALUE">
          <block id="V/FV`lCzd`zG*,HTH@#," type="math_number">
            <field name="NUM">0</field>
          </block>
        </value>
        <next>
          <block id="=N!Uk8jvC-2Am/B/qOMP" type="controls_whileUntil">
            <field name="MODE">WHILE</field>
            <value name="BOOL">
              <block id="ffmgT1|}9H{FlVCYKCKr" type="logic_compare">
                <field name="OP">LTE</field>
                <value name="A">
                  <block id="EPDEKK2dlo}u82tCmEz." type="variables_get">
                    <field id="664nQAmBX{%+.a4:(Uk}" name="VAR" variableType="">a</field>
                  </block>
                </value>
                <value name="B">
                  <block id="bL|PWGZ{m@/U{K=fb}hl" type="math_number">
                    <field name="NUM">200</field>
                  </block>
                </value>
              </block>
            </value>
            <statement name="DO">
              <block id="zn(1)2dfNr@]/-QO+DgF" type="variables_set">
                <field id="?YYJ/c@uyS!N3P+n3Oeq" name="VAR" variableType="">sum</field>
                <value name="VALUE">
                  <block id="FP#q]tn*fL1Qzb.{%7pE" type="math_arithmetic">
                    <field name="OP">ADD</field>
                    <value name="A">
                      <shadow id="|W=[Ypsp%1b)qzA2e-b@" type="math_number">
                        <field name="NUM">1</field>
                      </shadow>
                      <block id="*UDN^+6hVkdiP60R2aq*" type="variables_get">
                        <field id="?YYJ/c@uyS!N3P+n3Oeq" name="VAR" variableType="">sum</field>
                      </block>
                    </value>
                    <value name="B">
                      <shadow id="Blmv?y)7v^nAeu]sfU1p" type="math_number">
                        <field name="NUM">1</field>
                      </shadow>
                      <block id="Qw?jC:i;#LC:GBtO!|^n" type="variables_get">
                        <field id="664nQAmBX{%+.a4:(Uk}" name="VAR" variableType="">a</field>
                      </block>
                    </value>
                  </block>
                </value>
                <next>
                  <block id="ZaU_7C7sftC|_l5F9}{*" type="variables_set">
                    <field id="664nQAmBX{%+.a4:(Uk}" name="VAR" variableType="">a</field>
                    <value name="VALUE">
                      <block id="IEYgYS{.t^c+._OFwQd?" type="math_arithmetic">
                        <field name="OP">ADD</field>
                        <value name="A">
                          <shadow id="lq_GvoP_PluhiXxGUh%X" type="math_number">
                            <field name="NUM">1</field>
                          </shadow>
                          <block id="lL`}C40V=29[a0qj4qxg" type="variables_get">
                            <field id="664nQAmBX{%+.a4:(Uk}" name="VAR" variableType="">a</field>
                          </block>
                        </value>
                        <value name="B">
                          <shadow id="VShHV~7KB7-%1yBbv^]Y" type="math_number">
                            <field name="NUM">1</field>
                          </shadow>
                        </value>
                      </block>
                    </value>
                  </block>
                </next>
              </block>
            </statement>
            <next>
              <block id="wUqUd;[ToEFS=0OVaIXu" type="text_print">
                <value name="TEXT">
                  <shadow id="bjlY?!#]r/B;.%k?O_R/" type="text">
                    <field name="TEXT">abc</field>
                  </shadow>
                  <block id="F0t+boJG6ltk}df*w+-5" type="variables_get">
                    <field id="?YYJ/c@uyS!N3P+n3Oeq" name="VAR" variableType="">sum</field>
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