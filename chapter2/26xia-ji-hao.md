#夏及皓
---
###项目名称：将十进制数转化为二进制数
---
###项目内容：
1.界面和模块截图：  
![](/picture/xia-ji-hao/01.png)  
2.运行测试：  
![](/picture/xia-ji-hao/02.png)  
输入数字10:  
![](/picture/xia-ji-hao/03.png)  
输出10的二进制1010  
![](/picture/xia-ji-hao/04.png)  

----
###XML代码
```
<xml xmlns="http://www.w3.org/1999/xhtml">
  <variables>
    <variable type="" id="]82v9fXjXz1yXo~XZSoo">a</variable>
    <variable type="" id="lBZk]WbU)2^#LR?}u^8=">b</variable>
    <variable type="" id="dwzy[YDrmiQ3cdC5vaFq">c</variable>
    <variable type="" id="/noiW`oey}ckt:q`A(jl">i</variable>
  </variables>
  <block type="variables_set" id="ut9=Z#{C0=]vcH[GEU)~" x="488" y="88">
    <field name="VAR" id="]82v9fXjXz1yXo~XZSoo" variabletype="">a</field>
    <value name="VALUE">
      <block type="text_prompt_ext" id="j6hYX[@oKT?6)OPZ2U0,">
        <mutation type="NUMBER"></mutation>
        <field name="TYPE">NUMBER</field>
        <value name="TEXT">
          <shadow type="text" id="EuV?4dq-y|Z:#LzO0[)b">
            <field name="TEXT">abc</field>
          </shadow>
          <block type="text" id="@4nxRe%!kWfabI9loJA8">
            <field name="TEXT">请输入一个数字</field>
          </block>
        </value>
      </block>
    </value>
    <next>
      <block type="variables_set" id="*[}(l84RY!3IG~2hjG6N">
        <field name="VAR" id="dwzy[YDrmiQ3cdC5vaFq" variabletype="">c</field>
        <value name="VALUE">
          <block type="math_number" id="~v/Toz1%[(b)Z3[|cs~i">
            <field name="NUM">0</field>
          </block>
        </value>
        <next>
          <block type="variables_set" id="XTj^NcHCJKHGR)^/76l(">
            <field name="VAR" id="/noiW`oey}ckt:q`A(jl" variabletype="">i</field>
            <value name="VALUE">
              <block type="math_number" id="4+j}F2w[=W+F2N:/SVHH">
                <field name="NUM">0</field>
              </block>
            </value>
            <next>
              <block type="controls_whileUntil" id="j-F^]^~mCqb3i|*LA9:W">
                <field name="MODE">WHILE</field>
                <value name="BOOL">
                  <block type="logic_compare" id="V#vG3ZE:g4J(:#G}ND;B">
                    <field name="OP">NEQ</field>
                    <value name="A">
                      <block type="variables_get" id="M8H$P_JIA#$4:euv.f2D">
                        <field name="VAR" id="]82v9fXjXz1yXo~XZSoo" variabletype="">a</field>
                      </block>
                    </value>
                    <value name="B">
                      <block type="math_number" id="A15Uuh[tDN*(Y0mML@/`">
                        <field name="NUM">0</field>
                      </block>
                    </value>
                  </block>
                </value>
                <statement name="DO">
                  <block type="variables_set" id="Xabz*zyOy,(WhtdP!%ZB">
                    <field name="VAR" id="lBZk]WbU)2^#LR?}u^8=" variabletype="">b</field>
                    <value name="VALUE">
                      <block type="math_modulo" id="iE0DlBHu-3aV|2wSWbbD">
                        <value name="DIVIDEND">
                          <shadow type="math_number" id=")27ZQVSk{$WGIm|D~:Rx">
                            <field name="NUM">64</field>
                          </shadow>
                          <block type="variables_get" id="Xx$vjf{/2lKj;ZXa}2w.">
                            <field name="VAR" id="]82v9fXjXz1yXo~XZSoo" variabletype="">a</field>
                          </block>
                        </value>
                        <value name="DIVISOR">
                          <shadow type="math_number" id="unva)K.:xLt^GqrpY3*e">
                            <field name="NUM">10</field>
                          </shadow>
                          <block type="math_number" id="-6R{/Y:KYr}5G%%ezJ6b">
                            <field name="NUM">2</field>
                          </block>
                        </value>
                      </block>
                    </value>
                    <next>
                      <block type="variables_set" id="~-R6v{WM,+6Dy;@)PYU?">
                        <field name="VAR" id="dwzy[YDrmiQ3cdC5vaFq" variabletype="">c</field>
                        <value name="VALUE">
                          <block type="math_arithmetic" id=".a-28mYmp(LaG9GHd:B9">
                            <field name="OP">ADD</field>
                            <value name="A">
                              <shadow type="math_number" id="$;AdQ=*|IAsF,,D#jjK0">
                                <field name="NUM">1</field>
                              </shadow>
                              <block type="variables_get" 
id="^p69j~1?r+(,azBx#;[h">
                                <field name="VAR" id="dwzy[YDrmiQ3cdC5vaFq" variabletype="">c</field>
                              </block>
                            </value>
                            <value name="B">
                              <shadow type="math_number" id="ss_Fo}cyF!SxIQy*gU@B">
                                <field name="NUM">1</field>
                              </shadow>
                              <block type="math_arithmetic" id="b2*E2IxxbTvXCT#!p9~p">
                                <field name="OP">MULTIPLY</field>
                                <value name="A">
                                  <shadow type="math_number" id=";w}.~QI@oguAaKC:4bv?">
                                    <field name="NUM">1</field>
                                  </shadow>
                                  <block type="variables_get" id="$Sg!bt:$4!67bf`MGw=m">
                                    <field name="VAR" id="lBZk]WbU)2^#LR?}u^8=" variabletype="">b</field>
                                  </block>
                                </value>
                                <value name="B">
                                  <shadow type="math_number" id="g#UBUbY]@0():5KcV:Bj">
                                    <field name="NUM">1</field>
                                  </shadow>
                                  <block type="math_single" id="lN64Ovl9x8qe2#]F.IxX">
                                    <field name="OP">POW10</field>
                                    <value name="NUM">
                                      <shadow type="math_number" id="s9DT:WB%#*{11=ZK:u+P">
                                        <field name="NUM">9</field>
                                      </shadow>
                                      <block type="variables_get" id="%noLs`y|2Q]xk@Dzm0Hg">
                                        <field name="VAR" id="/noiW`oey}ckt:q`A(jl" variabletype="">i</field>
                                      </block>
                                    </value>
                                  </block>
                                </value>
                              </block>
                            </value>
                          </block>
                        </value>
                        <next>
                          <block type="variables_set" id="Wu!?hApsM-NlGqM-Z5,H">
                            <field name="VAR" id="]82v9fXjXz1yXo~XZSoo" variabletype="">a</field>
                            <value name="VALUE">
                              <block type="math_round" id="K@]E#1CXLO*U!8|)(2g(">
                                <field name="OP">ROUNDDOWN</field>
                                <value name="NUM">
                                  <shadow type="math_number" id="t,TVxxnmAEgcP8X{~)eE">
                                    <field name="NUM">3.1</field>
                                  </shadow>
                                  <block type="math_arithmetic" id="hd/8LT3H68@^Q$2;uM{n">
                                    <field name="OP">DIVIDE</field>
                                    <value name="A">
                                      <shadow type="math_number" id=";w}.~QI@oguAaKC:4bv?">
                                        <field name="NUM">1</field>
                                      </shadow>
                                      <block type="variables_get" id="K{dE8Y$qz-R.|*3Jv[d|">
                                        <field name="VAR" id="]82v9fXjXz1yXo~XZSoo" variabletype="">a</field>
                                      </block>
                                    </value>
                                    <value name="B">
                                      <shadow type="math_number" id="g#UBUbY]@0():5KcV:Bj">
                                        <field name="NUM">1</field>
                                      </shadow>
                                      <block type="math_number" id=":p6O5m5Z*NZ$45HC6lh7">
                                        <field name="NUM">2</field>
                                      </block>
                                    </value>
                                  </block>
                                </value>
                              </block>
                            </value>
                            <next>
                              <block type="variables_set" id="/#NW(+^u[}|a#5nfecW!">
                                <field name="VAR" id="/noiW`oey}ckt:q`A(jl" variabletype="">i</field>
                                <value name="VALUE">
                                  <block type="math_arithmetic" id="87*v-SDUSNc1#i@qFuUG">
                                    <field name="OP">ADD</field>
                                    <value name="A">
                                      <shadow type="math_number" id="uJ8%~J)$5TyEbWux8(-?">
                                        <field name="NUM">1</field>
                                      </shadow>
                                      <block type="variables_get" id="SWh_!n-0nwTc}Y9dQv@q">
                                        <field name="VAR" id="/noiW`oey}ckt:q`A(jl" variabletype="">i</field>
                                      </block>
                                    </value>
                                    <value name="B">
                                      <shadow type="math_number" id="I4s!gj|SfzIdLKBgw_o7">
                                        <field name="NUM">1</field>
                                      </shadow>
                                      <block type="math_number" id="ls83JiPb#sls*zk@1h.r">
                                        <field name="NUM">1</field>
                                      </block>
                                    </value>
                                  </block>
                                </value>
                              </block>
                            </next>
                          </block>
                        </next>
                      </block>
                    </next>
                  </block>
                </statement>
                <next>
 <block type="text_print" id="H-dTF85oD5KA0xCoO4mo">
                    <value name="TEXT">
                      <shadow type="text" id=":V73/BW+2)I)={(z1Ezk">
                        <field name="TEXT">abc</field>
                      </shadow>
                      <block type="variables_get" id="LB1T(vXLdiu]7jimI=nA">
                        <field name="VAR" id="dwzy[YDrmiQ3cdC5vaFq" variabletype="">c</field>
                      </block>
                    </value>
                  </block>
                </next>
              </block>
            </next>
          </block>
        </next>
      </block>
    </next>
  </block>
</xml>

```
