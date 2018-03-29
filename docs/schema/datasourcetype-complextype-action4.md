---


manager: soliver
ms.date: 3/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 71b6dbb4-e10c-8b08-c564-ce64ddb91382
---

![Collapse
section](../icons/collapse_all.gif "Collapse section")![Expand
section](../icons/expand_all.gif "Expand section")![](../icons/collapse_all.gif)![](../icons/expand_all.gif)![](../icons/dropdown.gif)![](../icons/dropdownHover.gif)![Copy
code](../icons/copycode.gif "Copy code")![Copy code
hover](../icons/copycodeHighlight.gif "Copy code hover")
<table>
<tbody>
<tr class="odd">
<td align="left"></td>
</tr>
</tbody>
</table>

Visual Basic  
C\#  
C++  
JavaScript  

<table>
<tbody>
<tr class="odd">
<td align="left"><span id="runningHeaderText"></span></td>
</tr>
<tr class="even">
<td align="left"># dataSourceType complexType (Action4)</td>
</tr>
<tr class="odd">
<td align="left"><span id="headfeedbackarea" class="feedbackhead"><a href="javascript:SubmitFeedback(&#39;docthis@Microsoft.com&#39;,&#39;&#39;,&#39;&#39;,&#39;&#39;,&#39;1.0.18082.1225&#39;,&#39;%0\dThank%20you%20for%20your%20feedback.%20The%20developer%20writing%20teams%20use%20your%20feedback%20to%20improve%20documentation.%20While%20we%20are%20reviewing%20your%20feedback,%20we%20may%20send%20you%20e-mail%20to%20ask%20for%20clarification%20or%20feedback%20on%20a%20solution.%20We%20do%20not%20use%20your%20e-mail%20address%20for%20any%20other%20purpose%20and%20we%20delete%20it%20after%20we%20finish%20our%20review.%0\AFor%20further%20information%20about%20the%20privacy%20policies%20of%20Microsoft,%20please%20see%20http://privacy.microsoft.com/en-us/default.aspx.%0\A%0\d&#39;,&#39;Customer%20feedback&#39;);">Send feedback</a></span></td>
</tr>
</tbody>
</table>

<table>
<colgroup>
<col width="100%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"></td>
</tr>
</tbody>
</table>

**Last modified:** March 09, 2015

**Applies to**: SharePoint Server 2013


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><p><span class="label">Namespace</span></p></td>
<td align="left"><p></p></td>
</tr>
<tr class="even">
<td align="left"><p><span class="label">Schema file</span></p></td>
<td align="left"><p>Actions4.xsd</p></td>
</tr>
<tr class="odd">
<td align="left"><p><span class="label">Extension base</span></p></td>
<td align="left"><p>None</p></td>
</tr>
</tbody>
</table>


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<span codelanguage="xmlLang"></span>
XML 
<span class="copyCode" onclick="CopyCode(this)"
onkeypress="CopyCode_CheckKey(this, event)"
onmouseover="ChangeCopyCodeIcon(this)"
onmouseout="ChangeCopyCodeIcon(this)" tabindex="0">![Copy
code](../icons/copycode.gif "Copy code")Copy code</span>
      
    <s:complexType name="dataSourceType">
        <s:sequence>
          <s:element name="SchemaSource">
            <s:complexType>
              <s:choice>
                <s:element name="Fields" minOccurs="0" maxOccurs="1">
                  <s:complexType>
                    <s:sequence>
                      <s:element name="Field" minOccurs="1" maxOccurs="unbounded">
                        <s:complexType>
                          <s:sequence>
                            <s:element name="CHOICES" minOccurs="0" maxOccurs="1">
                              <s:complexType>
                                <s:sequence>
                                  <s:element name="CHOICE" minOccurs="1" maxOccurs="unbounded">
                                    <s:complexType>
                                      <s:simpleContent>
                                        <s:extension base="s:string">
                                          <s:attribute name="DisplayName" type="s:string" />
                                        </s:extension>
                                      </s:simpleContent>
                                    </s:complexType>
                                  </s:element>
                                </s:sequence>
                              </s:complexType>
                            </s:element>
                          </s:sequence>
                          <s:attribute name="Name" type="s:string" />
                          <s:attribute name="DisplayName" type="s:string" />
                          <s:attribute name="Type" type="s:string" />
                        </s:complexType>
                      </s:element>
                    </s:sequence>
                  </s:complexType>
                </s:element>
                <s:element name="ContentType" minOccurs="0" maxOccurs="1">
                  <s:complexType>
                    <s:attribute name="IDFrom" type="s:string" />
                  </s:complexType>
                </s:element>
                <s:element name="Dictionary" minOccurs="0" maxOccurs="1">
                  <s:complexType>
                    <s:attribute name="ValueFrom" type="s:string" />
                  </s:complexType>
                </s:element>
                <s:element name="NestedInitiationFieldNodes" minOccurs="0" maxOccurs="1" />
              </s:choice>
            </s:complexType>
          </s:element>
          <s:element name="Evaluation">
            <s:complexType>
              <s:choice>
                <s:element name="ActivitySource">
                  <s:complexType>
                  </s:complexType>
                </s:element>
                <s:element name="HashtableSource">
                  <s:complexType>
                    <s:attribute name="HashtableFrom" type="s:string" />
                  </s:complexType>
                </s:element>
              </s:choice>
            </s:complexType>
          </s:element>
        </s:sequence>
        <s:attribute name="InternalName" type="s:string" use="required" />
        <s:attribute name="Name" type="s:string" use="required" />
        <s:attribute name="NameProperty" type="s:string" use="required" />
      </s:complexType>


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

If the schema defines specific requirements, such as **sequence**, **minOccurs**, **maxOccurs**, and **choice**, see the definition section.
class="keyword">sequence</span>, **minOccurs**,
**maxOccurs**, and <span
class="keyword">choice</span>, see the definition section.

### Child elements

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th align="left"><p>Element</p></th>
<th align="left"><p>Type</p></th>
<th align="left"><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p><a href="evaluation-element-datasourcetype-complextypeaction4.htm">Evaluation</a></p></td>
<td align="left"><p></p></td>
<td align="left"><p>Specifies whether values are retrieved from the data source fields of the parent action or composite step, or from a hash table.</p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="schemasource-element-datasourcetype-complextypeaction4.htm">SchemaSource</a></p></td>
<td align="left"><p></p></td>
<td align="left"><p>Specifies how data source fields are displayed.</p></td>
</tr>
</tbody>
</table>

### Attributes

<table>
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th align="left"><p>Attribute</p></th>
<th align="left"><p>Type</p></th>
<th align="left"><p>Required</p></th>
<th align="left"><p>Description</p></th>
<th align="left"><p>Possible values</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>InternalName</p></td>
<td align="left"><p>s:string</p></td>
<td align="left"><p>required</p></td>
<td align="left"><p></p></td>
<td align="left"><p>Values of the s:string type.</p></td>
</tr>
<tr class="even">
<td align="left"><p>Name</p></td>
<td align="left"><p>s:string</p></td>
<td align="left"><p>required</p></td>
<td align="left"><p></p></td>
<td align="left"><p>Values of the s:string type.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>NameProperty</p></td>
<td align="left"><p>s:string</p></td>
<td align="left"><p>required</p></td>
<td align="left"><p></p></td>
<td align="left"><p>Values of the s:string type.</p></td>
</tr>
</tbody>
</table>







