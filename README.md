# 6b
. Whether you're a seasoned chef or a home-cooking enthusiast, this recipe offers an approachable yet elevated culinary experience.
<?xml version = "1.0"?>
<?xml-stylesheet type = "text/xsl" href = "6b.xslt" ?>
<students>
   <VTU>
      <USN> 1RL01CS012 </USN>
      <name> GuruPrasad </name>
      <college> RLJIT </college>
      <branch> CSE</branch>
      <YOJ> 2006 </YOJ>
      <email> gp@gmail.com </email>
   </VTU>
   <VTU>
      <USN> 1Rl06CS053</USN>
      <name> SukruthGowda</name>
      <college> RLJIT </college>
      <branch>CSE </branch>
      <YOJ>2006</YOJ>
      <email>sukruth@gmail.com</email>
   </VTU>
   <VTU>
      <USN> 1RL06CS001</USN>
      <name>Abhishekbose</name>
      <college> RLJIT</college>
      <branch> CSE </branch>
      <YOJ>2006</YOJ>
      <email>abhishek@yahoo.com </email>
   </VTU>
</students>

XSLT

<?xml version = "1.0"?>
<xsl:stylesheet version = "1.0" xmlns:xsl = "http://www.w3.org/1999/XSL/Transform" xmlns = "http://www.w3.org/1999/xhtml" >
<xsl:template match = "students">
  <h2> VTU Students' Descriptions </h2>
  <xsl:for-each select = "VTU">
    <span style = "font-style: italic; color: blue;"> USN: </span>
<xsl:value-of select = "USN" /> <br />
    <span style = "font-style: italic; color: blue;"> Name: </span>
<xsl:value-of select = "name" /> <br />
    <span style = "font-style: italic; color: green;"> College: </span> 
<xsl:value-of select = "college" /> <br />
    <span style = "font-style: italic; color: red;"> Branch: </span> 
<xsl:value-of select = "branch" /> <br />
    <span style = "font-style: italic; color: yellow;"> Year of Join: </span> 
<xsl:value-of select = "YOJ" /> <br />
    <span style = "font-style: italic; color: blue;"> E-Mail: </span> 
<xsl:value-of select = "email" /> <br /> <br />
  </xsl:for-each>
 </xsl:template>
</xsl:stylesheet>
