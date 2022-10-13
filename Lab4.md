# GTECH785_Fall22

<b>SQL code and screenshots for Lab 4 </b><br>

<table>
  <tr>
    <th>SRID in PostGIS</th>
    <th>Spatial Reference System Name</th>
    <th>Datum Used</th>
    <th>Distance Unit</th>
    <th>Projection</th>
    <th>Applicable Regions/Areas</th>
  </tr>
  <tr>
    <td>Alfreds Futterkiste</td>
    <td>Maria Anders</td>
    <td>Germany</td>
  </tr>
  <tr>
    <td>Centro comercial Moctezuma</td>
    <td>Francisco Chang</td>
    <td>Mexico</td>
  </tr>
</table>

SRID in PostGIS	Spatial Reference System Name	Datum Used	Distance Unit	Projection 	Applicable Regions/Areas
4326	WGS 1984	WGS 84	Degree	Geographic coordinate system	World
3395	World Mercator	WGS 84	Degree	Mercator 1SP	World - between 80°S and 84°N
4269	NAD 83	NAD 83	Degree	Geographic coordinate system	North America
ESRI:102003	Albers for Contiguous US 	NAD 83	Degree	Albers Conic Equal Area	Contiguous USA
ESRI:102004	Lambert for Contiguous US 	NAD 83	Degree	Lambert Conformal Conic	Contiguous USA
3725 	UTM 18N 	NAD 83 2007	Degree	Transverse Mercator	USA, 72W to 78W. NY, PA, NJ, CT
3748	NAD83(HARN) / UTM zone 18N	NAD 83 HARN	Degree	Transverse Mercator	USA, 72W to 78W. NY, PA, NJ, CT
2263	SPCS Long Island	NAD 83	US Survey Foot	Lambert Conformal Conic	New York City, Nassau and Suffolk Counties
2831	SPCS Long Island	NAD 83 HARN	Meter	Lambert Conformal Conic	New York City, Nassau and Suffolk Counties
3627	SPCS Long Island	NAD 83 NSRS 2007	Meter	Lambert Conformal Conic	New York City, Nassau and Suffolk Counties
3628	NAD83(NSRS2007) / New York Long Island (ftUS)	NAD 83 NSRS 2007	US Survey Foot	Lambert Conformal Conic	New York City, Nassau and Suffolk Counties

<table class=MsoTableGrid border=1 cellspacing=0 cellpadding=0
 style='border-collapse:collapse;border:none;mso-border-alt:solid windowtext .5pt;
 mso-yfti-tbllook:1184;mso-padding-alt:0in 5.4pt 0in 5.4pt'>
 <tr style='mso-yfti-irow:0;mso-yfti-firstrow:yes;height:26.95pt'>
  <td width=105 valign=top style='width:78.65pt;border:solid windowtext 1.0pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt;height:26.95pt'>
  <p class=MsoNormal><b style='mso-bidi-font-weight:normal'><span
  style='mso-fareast-language:ZH-TW'>SRID in <span class=SpellE>PostGIS</span><i
  style='mso-bidi-font-style:normal'><o:p></o:p></i></span></b></p>
  </td>
  <td width=148 valign=top style='width:110.85pt;border:solid windowtext 1.0pt;
  border-left:none;mso-border-left-alt:solid windowtext .5pt;mso-border-alt:
  solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt;height:26.95pt'>
  <p class=MsoNormal><b style='mso-bidi-font-weight:normal'><span
  style='mso-fareast-language:ZH-TW'>Spatial Reference System Name<o:p></o:p></span></b></p>
  </td>
  <td width=74 valign=top style='width:55.3pt;border:solid windowtext 1.0pt;
  border-left:none;mso-border-left-alt:solid windowtext .5pt;mso-border-alt:
  solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt;height:26.95pt'>
  <p class=MsoNormal><b style='mso-bidi-font-weight:normal'><span
  style='mso-fareast-language:ZH-TW'>Datum Used<o:p></o:p></span></b></p>
  </td>
  <td width=77 valign=top style='width:58.0pt;border:solid windowtext 1.0pt;
  border-left:none;mso-border-left-alt:solid windowtext .5pt;mso-border-alt:
  solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt;height:26.95pt'>
  <p class=MsoNormal><b style='mso-bidi-font-weight:normal'><span
  style='mso-fareast-language:ZH-TW'>Distance Unit<o:p></o:p></span></b></p>
  </td>
  <td width=92 valign=top style='width:69.1pt;border:solid windowtext 1.0pt;
  border-left:none;mso-border-left-alt:solid windowtext .5pt;mso-border-alt:
  solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt;height:26.95pt'>
  <p class=MsoNormal><b style='mso-bidi-font-weight:normal'><span
  style='mso-fareast-language:ZH-TW'>Projection <o:p></o:p></span></b></p>
  </td>
  <td width=127 valign=top style='width:95.6pt;border:solid windowtext 1.0pt;
  border-left:none;mso-border-left-alt:solid windowtext .5pt;mso-border-alt:
  solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt;height:26.95pt'>
  <p class=MsoNormal><b style='mso-bidi-font-weight:normal'><span
  style='mso-fareast-language:ZH-TW'>Applicable Regions/Areas<o:p></o:p></span></b></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:1'>
  <td width=105 valign=top style='width:78.65pt;border:solid windowtext 1.0pt;
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt;
  padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>4326<o:p></o:p></span></p>
  </td>
  <td width=148 valign=top style='width:110.85pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>WGS 1984<o:p></o:p></span></p>
  </td>
  <td width=74 valign=top style='width:55.3pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>WGS 84<o:p></o:p></span></p>
  </td>
  <td width=77 valign=top style='width:58.0pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>Degree<o:p></o:p></span></p>
  </td>
  <td width=92 valign=top style='width:69.1pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>Geographic
  coordinate system<o:p></o:p></span></p>
  </td>
  <td width=127 valign=top style='width:95.6pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>World<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:2'>
  <td width=105 valign=top style='width:78.65pt;border:solid windowtext 1.0pt;
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt;
  padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>3395<o:p></o:p></span></p>
  </td>
  <td width=148 valign=top style='width:110.85pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>World Mercator<o:p></o:p></span></p>
  </td>
  <td width=74 valign=top style='width:55.3pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>WGS 84<o:p></o:p></span></p>
  </td>
  <td width=77 valign=top style='width:58.0pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>Degree<o:p></o:p></span></p>
  </td>
  <td width=92 valign=top style='width:69.1pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>Mercator 1SP<o:p></o:p></span></p>
  </td>
  <td width=127 valign=top style='width:95.6pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>World - between
  80°S and 84°N<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:3'>
  <td width=105 valign=top style='width:78.65pt;border:solid windowtext 1.0pt;
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt;
  padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>4269<o:p></o:p></span></p>
  </td>
  <td width=148 valign=top style='width:110.85pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>NAD 83<o:p></o:p></span></p>
  </td>
  <td width=74 valign=top style='width:55.3pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>NAD 83<o:p></o:p></span></p>
  </td>
  <td width=77 valign=top style='width:58.0pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>Degree<o:p></o:p></span></p>
  </td>
  <td width=92 valign=top style='width:69.1pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>Geographic
  coordinate system<o:p></o:p></span></p>
  </td>
  <td width=127 valign=top style='width:95.6pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>North America<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:4'>
  <td width=105 valign=top style='width:78.65pt;border:solid windowtext 1.0pt;
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt;
  padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>ESRI:102003<o:p></o:p></span></p>
  </td>
  <td width=148 valign=top style='width:110.85pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>Albers for
  Contiguous US <o:p></o:p></span></p>
  </td>
  <td width=74 valign=top style='width:55.3pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>NAD 83<o:p></o:p></span></p>
  </td>
  <td width=77 valign=top style='width:58.0pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>Degree<o:p></o:p></span></p>
  </td>
  <td width=92 valign=top style='width:69.1pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>Albers Conic
  Equal Area<o:p></o:p></span></p>
  </td>
  <td width=127 valign=top style='width:95.6pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>Contiguous USA<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:5'>
  <td width=105 valign=top style='width:78.65pt;border:solid windowtext 1.0pt;
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt;
  padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>ESRI:102004<o:p></o:p></span></p>
  </td>
  <td width=148 valign=top style='width:110.85pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>Lambert for
  Contiguous US <o:p></o:p></span></p>
  </td>
  <td width=74 valign=top style='width:55.3pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>NAD 83<o:p></o:p></span></p>
  </td>
  <td width=77 valign=top style='width:58.0pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>Degree<o:p></o:p></span></p>
  </td>
  <td width=92 valign=top style='width:69.1pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>Lambert Conformal
  Conic<o:p></o:p></span></p>
  </td>
  <td width=127 valign=top style='width:95.6pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>Contiguous USA<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:6'>
  <td width=105 valign=top style='width:78.65pt;border:solid windowtext 1.0pt;
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt;
  padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>3725 <o:p></o:p></span></p>
  </td>
  <td width=148 valign=top style='width:110.85pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>UTM 18N <o:p></o:p></span></p>
  </td>
  <td width=74 valign=top style='width:55.3pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>NAD 83 2007<o:p></o:p></span></p>
  </td>
  <td width=77 valign=top style='width:58.0pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>Degree<o:p></o:p></span></p>
  </td>
  <td width=92 valign=top style='width:69.1pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>Transverse
  Mercator<o:p></o:p></span></p>
  </td>
  <td width=127 valign=top style='width:95.6pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>USA, 72W to 78W.
  NY, PA, NJ, CT<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:7'>
  <td width=105 valign=top style='width:78.65pt;border:solid windowtext 1.0pt;
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt;
  padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>3748<o:p></o:p></span></p>
  </td>
  <td width=148 valign=top style='width:110.85pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>NAD83(HARN) / UTM
  zone 18N<o:p></o:p></span></p>
  </td>
  <td width=74 valign=top style='width:55.3pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>NAD 83 HARN<o:p></o:p></span></p>
  </td>
  <td width=77 valign=top style='width:58.0pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>Degree<o:p></o:p></span></p>
  </td>
  <td width=92 valign=top style='width:69.1pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>Transverse
  Mercator<o:p></o:p></span></p>
  </td>
  <td width=127 valign=top style='width:95.6pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>USA, 72W to 78W.
  NY, PA, NJ, CT<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:8'>
  <td width=105 valign=top style='width:78.65pt;border:solid windowtext 1.0pt;
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt;
  padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>2263<o:p></o:p></span></p>
  </td>
  <td width=148 valign=top style='width:110.85pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>SPCS Long Island<o:p></o:p></span></p>
  </td>
  <td width=74 valign=top style='width:55.3pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>NAD 83<o:p></o:p></span></p>
  </td>
  <td width=77 valign=top style='width:58.0pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>US Survey Foot<o:p></o:p></span></p>
  </td>
  <td width=92 valign=top style='width:69.1pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>Lambert Conformal
  Conic<o:p></o:p></span></p>
  </td>
  <td width=127 valign=top style='width:95.6pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>New York City, <span
  class=GramE>Nassau</span> and Suffolk Counties<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:9'>
  <td width=105 valign=top style='width:78.65pt;border:solid windowtext 1.0pt;
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt;
  padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>2831<o:p></o:p></span></p>
  </td>
  <td width=148 valign=top style='width:110.85pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>SPCS Long Island<o:p></o:p></span></p>
  </td>
  <td width=74 valign=top style='width:55.3pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>NAD 83 HARN<o:p></o:p></span></p>
  </td>
  <td width=77 valign=top style='width:58.0pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>Meter<o:p></o:p></span></p>
  </td>
  <td width=92 valign=top style='width:69.1pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>Lambert Conformal
  Conic<o:p></o:p></span></p>
  </td>
  <td width=127 valign=top style='width:95.6pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>New York City, <span
  class=GramE>Nassau</span> and Suffolk Counties<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:10'>
  <td width=105 valign=top style='width:78.65pt;border:solid windowtext 1.0pt;
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt;
  padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>3627<o:p></o:p></span></p>
  </td>
  <td width=148 valign=top style='width:110.85pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>SPCS Long Island<o:p></o:p></span></p>
  </td>
  <td width=74 valign=top style='width:55.3pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>NAD 83 NSRS 2007<o:p></o:p></span></p>
  </td>
  <td width=77 valign=top style='width:58.0pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>Meter<o:p></o:p></span></p>
  </td>
  <td width=92 valign=top style='width:69.1pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>Lambert Conformal
  Conic<o:p></o:p></span></p>
  </td>
  <td width=127 valign=top style='width:95.6pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>New York City, <span
  class=GramE>Nassau</span> and Suffolk Counties<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:11;mso-yfti-lastrow:yes'>
  <td width=105 valign=top style='width:78.65pt;border:solid windowtext 1.0pt;
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt;
  padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>3628<o:p></o:p></span></p>
  </td>
  <td width=148 valign=top style='width:110.85pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>NAD83(NSRS2007) /
  New York Long Island (<span class=SpellE>ftUS</span>)<o:p></o:p></span></p>
  </td>
  <td width=74 valign=top style='width:55.3pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>NAD 83 NSRS 2007<o:p></o:p></span></p>
  </td>
  <td width=77 valign=top style='width:58.0pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>US Survey Foot<o:p></o:p></span></p>
  </td>
  <td width=92 valign=top style='width:69.1pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>Lambert Conformal
  Conic<o:p></o:p></span></p>
  </td>
  <td width=127 valign=top style='width:95.6pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt'>
  <p class=MsoNormal><span style='mso-fareast-language:ZH-TW'>New York City, <span
  class=GramE>Nassau</span> and Suffolk Counties<o:p></o:p></span></p>
  </td>
 </tr>
</table>




