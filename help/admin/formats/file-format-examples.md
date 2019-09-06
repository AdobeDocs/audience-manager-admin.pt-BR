---
description: Exemplos de como macros são usadas para criar modelos de arquivo de saída e FTP.
seo-description: Exemplos de como macros são usadas para criar modelos de arquivo de saída e FTP.
seo-title: Exemplos de formato de arquivo
title: Exemplos de formato de arquivo
uuid: f 00 d 431 d -7 e 43-457 a-b 633-c 79 cbc 4 c 8 f 10
translation-type: tm+mt
source-git-commit: 4c6d1752ff10d2d3d12cab88e823f25f5ef4fcd0

---


# Exemplos de formato de arquivo {#file-format-macro-examples}

Exemplos de como macros são usadas para criar modelos de saída e [!DNL FTP] de arquivo.

>[!NOTE]
>
>Nas tabelas, **o tipo de negrito** identifica cada macro com sua saída relacionada. Para os exemplos de formato, os símbolos &lt; &gt; foram adicionados para ajudar a separar visualmente cada macro.

## Macros comuns {#common-macros}

Essas macros podem ser usadas em qualquer campo de formato. Consulte Macros de formato [de arquivo](../formats/file-formats.md) para obter uma lista completa e definições.

<table id="table_B5073597219B470298EE614902DACAE8"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Macro </th> 
   <th colname="col2" class="entry"> Exemplos de formato e saída </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <code>DPID </code> </p> </td> 
   <td colname="col2"> <p>Formato: <code>&lt; SYNC_ TYPE &gt;_ &lt; ORDER_ ID &gt;_ &lt; DPID &gt;_ &lt; SYNC_ MODE &gt;_ &lt; TIMESTAMP &gt;. sync </code> </p> <p>Saída: <code>ftp_ 215_ 888_ iter_ 1449756724. sync </code> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>MASTER_ DPID </code> </p> </td> 
   <td colname="col2"> <p>Formato: <code>&lt; SYNC_ TYPE &gt;_ &lt; ORDER_ ID &gt;_ &lt; DPID &gt;_ &lt; MASTER_ DPID &gt;_ &lt; SYNC_ MODE &gt;_ &lt; TIMESTAMP &gt;. sync </code> </p> <p>Saída: <code>ftp_ 215_ 888_ 20915_ iter_ 1449756724. sync </code> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>ORDER_ ID </code> </p> </td> 
   <td colname="col2"> <p>Formato: <code>&lt; SYNC_ TYPE &gt;_ &lt; ORDER_ ID &gt;_ &lt; DPID &gt;_ &lt; SYNC_ MODE &gt;_ &lt; TIMESTAMP &gt;. sync </code> </p> <p>Saída: <code>ftp_ 215_ 888_ iter_ 1449756724. sync </code> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>SYNC_ MODE </code> </p> </td> 
   <td colname="col2"> <p>Formato: <code>&lt; SYNC_ TYPE &gt;_ &lt; ORDER_ ID &gt;_ &lt; DPID &gt;_ &lt; SYNC_ MODE &gt;_ &lt; TIMESTAMP &gt;. sync </code> </p> <p>Saída: 
     <ul id="ul_F63D7B78AF1246639D6ED85C1621B17C"> 
      <li id="li_4D0D7B4D047345FE861FCBA2BD0408ED">Total: <code>ftp_ 215_ 888_ full_ 1449756724. sync </code> </li> 
      <li id="li_23F4D1F6B2784E599EDA29AA457327E6">Incremental: <code>ftp_ 215_ 888_ iter_ 1449756724. sync </code> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>SYNC_ TYPE </code> </p> </td> 
   <td colname="col2"> <p>Formato: <code>&lt; SYNC_ TYPE &gt;_ &lt; ORDER_ ID &gt;_ &lt; DPID &gt;_ &lt; SYNC_ MODE &gt;_ &lt; TIMESTAMP &gt;. sync </code> </p> <p>Saída: 
     <ul id="ul_11B14E740E40474F8302BDB809C428FE"> 
      <li id="li_54A3EAA468B44AC8B2528F855E03D04B">FTP: <code>ftp_ 215_ 888_ iter_ 1449756724. sync </code> </li> 
      <li id="li_93468C56B661463CA7F62B1F5D3A53FF">https: <code>http_ 215_ 888_ iter_ 1449756724. sync </code> </li> 
      <li id="li_8A204C7BEDBC41C096FE953B5F827DEC">S 3: <code>s 3_ 215_ 888_ iter_ 1449756724. sync </code> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>TIMESTAMP </code> </p> </td> 
   <td colname="col2"> <p>Formato: <code>&lt; SYNC_ TYPE &gt;_ &lt; ORDER_ ID &gt;_ &lt; DPID &gt;_ &lt; SYNC_ MODE &gt;_ &lt; TIMESTAMP &gt;. sync </code> </p> <p>Saída: <code>ftp_ 215_ 888_ iter_ 1449756724. sync </code> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Macros de campo de cabeçalho {#header-field-macros}

Macros usadas apenas em campos de cabeçalho. Consulte Macros de formato [de arquivo](../formats/file-formats.md) para obter uma lista completa e definições.

<table id="table_ABC31B3D660D47969E111EBC734D5BBC"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Macro </th> 
   <th colname="col2" class="entry"> Exemplos de formato e saída </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <code>TAB </code> </p> </td> 
   <td colname="col2"> <p>Formato: <code>&lt; ORDER_ ID &gt; &lt; TAB &gt; &lt; SYNC_ TYPE &gt; </code> </p> <p>Saída: <code>888 full. sync </code> </p> <p>Na saída, o caractere da guia não impressão separa cada elemento. </p> </td>
  </tr>
 </tbody>
</table>

## Macros de linha de dados {#data-row-macros}

Macros usadas apenas em campos de cabeçalho. Consulte Macros de formato [de arquivo](../formats/file-formats.md) para obter uma lista completa e definições.

<table id="table_408C6DD2B9D54550B003EAC93562E64F"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Macro </th> 
   <th colname="col2" class="entry"> Exemplos de formato e saída </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <code>DP_ UUID </code> </p> </td> 
   <td colname="col2"> <p>Formato: <code>&lt; DP_ UUID &gt; &lt; TAB &gt; &lt; DP_ UUID_ LIST; separator = TAB &gt; </code> </p> <p>Saída: <code>123456 UUID 1 UUID 2 UUID 3 </code> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>DP_ UUID_ LIST </code> </p> </td> 
   <td colname="col2"> <p>Formato: <code>&lt; DP_ UUID &gt; &lt; TAB &gt; &lt; DP_ UUID_ LIST; separator = TAB &gt; </code> </p> <p>Saída: <code>123456 UUID 1 UUID 2 UUID 3 </code> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>SEGMENT_ LIST &amp; &amp; REMOVED_ SEGMENT_ LIST </code> </p> </td> 
   <td colname="col2"> <p>Este exemplo cria um formato que retorna segmentos removidos em um feed servidor para servidor. </p> <p> 
     <code>{"Advertiserid": " &lt; PIDALIAS &gt; "," datacenterid ": 2, "TDID": " &lt; DP_ UUID &gt; ", 
 " Dados ": [&lt; SEGMENT_ LIST: {seg|&lt; OPEN_ CURLY_ BRACKET &gt; "Name": " &lt; seg. alias &gt; " &lt; CLOSE_ CURLY_ BRACKET &gt;}; 
 separator = "," &gt; &lt; if (SEGMENT_ LIST &amp; &amp; &amp;_ SEGMENT_ LIST) &gt; &lt; VÍRA &gt; &lt; endif &gt; 
 &lt; REMOVED_ SEGMENT_ LIST: {seg|&lt; OPEN_ CURLY_ BRACKET &gt; "Name": " &lt; seg. alias &gt; ", 
 " Ttlinminutes ": 0 &lt; CLOSE_ CURLY_ BRACKET &gt;}; separator = "," &gt;]} </code>
  </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>SEGMENT_ LIST </code> </p> </td> 
   <td colname="col2"> <p>Formato: <code>&lt; DP_ UUID &gt; &lt; SEGMENT_ LIST &gt;; separator = "" &gt; </code> </p> <p>Saída: <code>123456 105955 101183 101180 101179 </code> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>SET_ ATTRIBUTES </code> </p> </td> 
   <td colname="col2"> <p>Formato: <code>&lt; PID &gt; &lt; TAB &gt; &lt; UUID &gt; &lt; TAB &gt; &lt; DP_ UUID &gt; &lt; TAB &gt; &lt; SET_ ATTRIBUTES &gt; &lt; TAB &gt; &lt; OPT_ OUT &gt; &lt; TAB &gt; &lt; SEGMENT_ LIST: {seg|&lt; seg. type &gt;, &lt; seg. alias &gt;, &lt; OUTPUT_ ATTRIBUTE_ VALUE &gt;, &lt; seg. lastupdatetime &gt; &amp;} &gt; </code> </p> <p>Saída: <code>1159 00088008579683653741516297509717335000 17 t 0 aj 01 b,103714,1,03714,1,13441&amp; 4661000 &amp; 5,103713,1,1343250661000 </code> </p> </td>
  </tr>
  <tr> 
   <td colname="col1"> <p> <code>TAB </code> </p> </td> 
   <td colname="col2"> <p>Formato: <code>&lt; DP_ UUID &gt; &lt; TAB &gt; &lt; DP_ UUID_ LIST; separator = TAB &gt; </code> </p> <p>Saída: <code>123456 UUID 1 UUID 2 UUID 3 </code> </p> <p>Na saída, o caractere da guia não impressão separa cada elemento. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>TRAIT_ LIST </code> </p> </td> 
   <td colname="col2"> <p>Formato: <code>&lt; PID &gt; &lt; TAB &gt; &lt; DP_ UUID &gt; &lt; TAB &gt; &lt; SET_ ATTRIBUTES &gt; &lt; TAB &gt; &lt; TRAIT_ LIST; separator = «|» &gt; </code> </p> <p>Saída: <code>1131 12345 1 123|456|789 </code> </p> </td> 
  </tr> 
 </tbody> 
</table>
