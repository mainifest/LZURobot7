#武山权
---
###项目名称：找出一类具有某种性质的五位数
---
###项目内容：
我们可以假设一个5位数，从左数第一个数能被9整除，从左数前2位数能被8整除，以此类推。程序以枚举法找到它。  
![](/picture/wu-shan-quan/01.png)  
可得下方四个数字  
![](/picture/wu-shan-quan/02.png)  

---
###XML代码
```
<xml xmlns="http://www.w3.org/1999/xhtml">
  <variables>
    <variable type="" id="2uYZ0(k^D3|htcBmRIh+">i</variable>
    <variable type="" id="8YYgV(h+_xLXDj;ia]`d">a</variable>
    <variable type="" id="YN!GDNP~.KxXEpl7$$xG">b</variable>
    <variable type="" id="-HOW11d7M{nd;9!]zM2;">c</variable>
    <variable type="" id="5@H]wgF/8L?!]{?P8]^X">d</variable>
    <variable type="" id="uf2wC+3Gp$43GbEL*imB">e</variable>
  </variables>
  <block type="controls_for" id="m~Qg%,RCMB!IQOhc/Vpv" x="213" y="138">
    <field name="VAR" id="2uYZ0(k^D3|htcBmRIh+" variabletype="">i</field>
    <value name="FROM">
      <shadow type="math_number" id="z_0C~I%4U#:E]SEgTQvi">
        <field name="NUM">10000</field>
      </shadow>
    </value>
    <value name="TO">
      <shadow type="math_number" id="^nAcbk0p0L6~-Ui0P_z+">
        <field name="NUM">99999</field>
      </shadow>
    </value>
    <value name="BY">
      <shadow type="math_number" id="}},6-4Za(^kc0RGgaX~*">
        <field name="NUM">1</field>
      </shadow>
    </value>
    <statement name="DO">
      <block type="variables_set" id="Cjlbn+t(w3F)m:2]x`_j">
        <field name="VAR" id="8YYgV(h+_xLXDj;ia]`d" variabletype="">a</field>
        <value name="VALUE">
          <block type="math_round" id="bY]GcJFiviHa0_HyuhY-">
            <field name="OP">ROUNDDOWN</field>
            <value name="NUM">
              <shadow type="math_number" id="8}gsQwiaHjV]R5`=P=cJ">
                <field name="NUM">3.1</field>
              </shadow>
              <block type="math_arithmetic" id="=APx{MMnoWv;k5sbJ)pD">
                <field name="OP">DIVIDE</field>
                <value name="A">
                  <shadow type="math_number" id="EeO!z)T,xvXvcCt~5@]v">
                    <field name="NUM">1</field>
                  </shadow>
                  <block type="variables_get" id="tSU(p|]%.iDrpEs=bXU*">
                    <field name="VAR" id="2uYZ0(k^D3|htcBmRIh+" variabletype="">i</field>
                  </block>
                </value>
                <value name="B">
                  <shadow type="math_number" id="]7mF-{(/H?V%t7ni!r+l">
                    <field name="NUM">10000</field>
                  </shadow>
                </value>
              </block>
            </value>
          </block>
        </value>
        <next>
          <block type="controls_if" id="q!67;G$kX?}BhNo[VZio">
            <value name="IF0">
              <block type="math_number_property" id="+3x!Kcu^PpeRQCz=rry`">
                <mutation divisor_input="false"></mutation>
                <field name="PROPERTY">WHOLE</field>
                <value name="NUMBER_TO_CHECK">
                  <shadow type="math_number" id="1~xDx+g#.`]jgR,Nk]VJ">
                    <field name="NUM">0</field>
                  </shadow>
                  <block type="math_arithmetic" id="]z@o9fFoJtC?-Wk#cr{N">
                    <field name="OP">DIVIDE</field>
                    <value name="A">
                      <shadow type="math_number" id="UP5OcE!ml@Y/4Hmd7]Ci">
                        <field name="NUM">1</field>
                      </shadow>
                      <block type="variables_get" id="Fs;u#-C*s|.h[d-CGb]W">
                        <field name="VAR" id="8YYgV(h+_xLXDj;ia]`d" variabletype="">a</field>
                      </block>
                    </value>
                    <value name="B">
                      <shadow type="math_number" id="x!,;7e`p1mp#qQ(oo`wY">
                        <field name="NUM">9</field>
                      </shadow>
                    </value>
                  </block>
                </value>
              </block>
            </value>
            <statement name="DO0">
              <block type="variables_set" id="]R2)bACqO?$+BSSR8#z`">
                <field name="VAR" id="YN!GDNP~.KxXEpl7$$xG" variabletype="">b</field>
                <value name="VALUE">
                  <block type="math_round" id="rI{0*XZ(It95ZaEPT4R#">
                    <field name="OP">ROUND</field>
                    <value name="NUM">
                      <shadow type="math_number" id="N[jGm7bU2b#k2bR0nR`I">
                        <field name="NUM">3.1</field>
                      </shadow>
                      <block type="math_arithmetic" id="~rxME!MxpMB0VR`)95X0">
                        <field name="OP">DIVIDE</field>
                        <value name="A">
                          <shadow type="math_number" id="fx!4d3L0*+%X`MAA]tZ7">
                            <field name="NUM">1</field>
                          </shadow>
                          <block type="variables_get" id="=Zaw07/Y6_0~%r|kckkT">
                            <field name="VAR" id="2uYZ0(k^D3|htcBmRIh+" variabletype="">i</field>
                          </block>
                        </value>
                        <value name="B">
                          <shadow type="math_number" id=")iP2nO7Z/^s(4ElmxWHW">
                            <field name="NUM">1000</field>
                          </shadow>
                        </value>
                      </block>
                    </value>
                  </block>
                </value>
                <next>
                  <block type="controls_if" id="n[D+eZCaqV,yf?}fAl8#">
                    <value name="IF0">
                      <block type="math_number_property" id="@v5E_n{1@saKRbAkQNG.">
                        <mutation divisor_input="false"></mutation>
                        <field name="PROPERTY">WHOLE</field>
                        <value name="NUMBER_TO_CHECK">
                          <shadow type="math_number" id="$cBP5b/WtQ}b-DQY~D]K">
                            <field name="NUM">0</field>
                          </shadow>
                          <block type="math_arithmetic" id="XbuIl6WY0la1WOrV/L6F">
                            <field name="OP">DIVIDE</field>
                            <value name="A">
                              <shadow type="math_number" id="LFFci~^JcN74tbmz6)p9">
                                <field name="NUM">1</field>
                              </shadow>
                              <block type="variables_get" id="oVN}#AWut7FzwJ#O1y:$">
                                <field name="VAR" id="YN!GDNP~.KxXEpl7$$xG" variabletype="">b</field>
                              </block>
                            </value>
                            <value name="B">
                              <shadow type="math_number" id="7rNd)ZVMIgHRb[#{7{w)">
                                <field name="NUM">8</field>
                              </shadow>
                            </value>
                          </block>
                        </value>
                      </block>
                    </value>
                    <statement name="DO0">
                      <block type="variables_set" id="DQu/@uMkd2JB%7mHiWGt">
                        <field name="VAR" id="-HOW11d7M{nd;9!]zM2;" variabletype="">c</field>
                        <value name="VALUE">
                          <block type="math_round" id="urso%%cCf3WNN6WV1$?.">
                            <field name="OP">ROUND</field>
                            <value name="NUM">
                              <shadow type="math_number" id="A5a}!p/G8X9=J$yYICg5">
                                <field name="NUM">3.1</field>
                              </shadow>
                              <block type="math_arithmetic" id="d)#?ic*QR$5k%fbhYler">
                                <field name="OP">DIVIDE</field>
                                <value name="A">
                                  <shadow type="math_number" id="vk`]e3L^KjKAHJYBM#+p">
                                    <field name="NUM">1</field>
                                  </shadow>
                                  <block type="variables_get" id="l]fwCuuI/4xx]/un#pOk">
                                    <field name="VAR" id="2uYZ0(k^D3|htcBmRIh+" variabletype="">i</field>
                                  </block>
                                </value>
                                <value name="B">
                                  <shadow type="math_number" id="!^7SsxiZ5hQO,:Bqa/lO">
                                    <field name="NUM">100</field>
                                  </shadow>
                                </value>
                              </block>
                            </value>
                          </block>
                        </value>
                        <next>
                          <block type="controls_if" id="h7$}%O9gE2fQ7#TwCOiM">
                            <value name="IF0">
                              <block type="math_number_property" id="wh^V*Po$}!E?dF5I4(oc">
                                <mutation divisor_input="false"></mutation>
                                <field name="PROPERTY">WHOLE</field>
                                <value name="NUMBER_TO_CHECK">
                                  <shadow type="math_number" id="Mr0v7K76^I#XUrM_l~^a">
                                    <field name="NUM">0</field>
                                  </shadow>
                                  <block type="math_arithmetic" id=",ed6]{?nhRLUK=uWC|cO">
                                    <field name="OP">DIVIDE</field>
                                    <value name="A">
                                      <shadow type="math_number" id="S2CpR;:yrW[h~1j|yM3;">
                                        <field name="NUM">1</field>
                                      </shadow>
                                      <block type="variables_get" id="2:QH`:N7[S~o@8wb*@J=">
                                        <field name="VAR" id="-HOW11d7M{nd;9!]zM2;" variabletype="">c</field>
                                      </block>
                                    </value>
                                    <value name="B">
                                      <shadow type="math_number" id="l@gPPDR8Pa_iLBO|Ce0+">
                                        <field name="NUM">7</field>
                                      </shadow>
                                    </value>
                                  </block>
                                </value>
                              </block>
                            </value>
                            <statement name="DO0">
                              <block type="variables_set" id="$^?.ob+7RetEm(Y7)Gn7">
                                <field name="VAR" id="5@H]wgF/8L?!]{?P8]^X" variabletype="">d</field>
                                <value name="VALUE">
                                  <block type="math_round" id="[5u6.RJSjHlEd!k_HHuZ">
                                    <field name="OP">ROUND</field>
                                    <value name="NUM">
                                      <shadow type="math_number" id="g}.h!X+KJ-iE=zTSY2fa">
                                        <field name="NUM">3.1</field>
                                      </shadow>
                                      <block type="math_arithmetic" id="OYAO!o[uw$$=g)uq)vwT">
                                        <field name="OP">DIVIDE</field>
                                        <value name="A">
                                          <shadow type="math_number" id="t$wDF)%VS$MZJCBO,ubf">
                                            <field name="NUM">1</field>
                                          </shadow>
                                          <block type="variables_get" id="Xho,v|X;4obztyHI`C*A">
                                            <field name="VAR" id="2uYZ0(k^D3|htcBmRIh+" variabletype="">i</field>
                                          </block>
                                        </value>
                                        <value name="B">
                                          <shadow type="math_number" id="i7/3vu$yUcvFal|){hc}">
                                            <field name="NUM">10</field>
                                          </shadow>
                                        </value>
                                      </block>
                                    </value>
                                  </block>
                                </value>
                                <next>
                                  <block type="controls_if" id="zEash`r9W?~wW:,+7md-">
                                    <value name="IF0">
                                      <block type="math_number_property" id="TxwVy.KDHJ}tQD|?c10G">
                                        <mutation divisor_input="false"></mutation>
                                        <field name="PROPERTY">WHOLE</field>
                                        <value name="NUMBER_TO_CHECK">
                                          <shadow type="math_number" id="Ct?FR?H7-ykS=!Xp+0-M">
                                            <field name="NUM">0</field>
                                          </shadow>
                                          <block type="math_arithmetic" id="VOR5hR?KE6Ho1Y:Hb]zX">
                                            <field name="OP">DIVIDE</field>
                                            <value name="A">
                                              <shadow type="math_number" id="YzPT#;0?%^py_`X)zBPJ">
                                                <field name="NUM">1</field>
                                              </shadow>
                                              <block type="variables_get" id="!j3V|N,xoZT0A@.0UK0d">
                                                <field name="VAR" id="5@H]wgF/8L?!]{?P8]^X" variabletype="">d</field>
                                              </block>
                                            </value>
                                            <value name="B">
                                              <shadow type="math_number" id="yDd:`%C%_x50orCP8SYR">
                                                <field name="NUM">6</field>
                                              </shadow>
                                            </value>
                                          </block>
                                        </value>
                                      </block>
                                    </value>
                                    <statement name="DO0">
                                      <block type="controls_if" id="dHh#M8QSicwWe=u(L?IQ">
                                        <value name="IF0">
                                          <block type="math_number_property" id="a`:JpCe2W2*YBsdT4@Ul">
                                            <mutation divisor_input="false"></mutation>
                                            <field name="PROPERTY">WHOLE</field>
                                            <value name="NUMBER_TO_CHECK">
                                              <shadow type="math_number" id="2L}r~bOO|P[=c56-=6$D">
                                                <field name="NUM">0</field>
                                              </shadow>
                                              <block type="math_arithmetic" id="djL}Sp1CV09pFm-=7srL">
                                                <field name="OP">DIVIDE</field>
                                                <value name="A">
                                                  <shadow type="math_number" id="(49~L$mW_5$Wc7!7,/pC">
                                                    <field name="NUM">1</field>
                                                  </shadow>
                                                  <block type="variables_get" id="Lml{I_Ea~@nd,?Buh|lH">
                                                    <field name="VAR" id="2uYZ0(k^D3|htcBmRIh+" variabletype="">i</field>
                                                  </block>
                                                </value>
                                                <value name="B">
                                                  <shadow type="math_number" id="=0gra%lvBJ]*4_THD{d#">
                                                    <field name="NUM">5</field>
                                                  </shadow>
                                                </value>
                                              </block>
                                            </value>
                                          </block>
                                        </value>
                                        <statement name="DO0">
                                          <block type="text_print" id="CQIZZDwj/8m*hA*pAmQD">
                                            <value name="TEXT">
                                              <shadow type="text" id="CPd*L{6.0aV`MZ`]-ynL">
                                                <field name="TEXT">abc</field>
                                              </shadow>
                                              <block type="variables_get" id="FiJ@$EF5IZpnjV.hjzB$">
                                                <field name="VAR" id="2uYZ0(k^D3|htcBmRIh+" variabletype="">i</field>
                                              </block>
                                            </value>
                                          </block>
                                        </statement>
                                      </block>
                                    </statement>
                                  </block>
                                </next>
                              </block>
                            </statement>
                          </block>
                        </next>
                      </block>
                    </statement>
                  </block>
                </next>
              </block>
            </statement>
          </block>
        </next>
      </block>
    </statement>
  </block>
</xml>

```
