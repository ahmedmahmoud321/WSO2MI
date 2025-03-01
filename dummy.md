#### This crap to be studied later

```text
### XSLT

#### What is XSL?

XSL (eXtensible Stylesheet Language) is a language for transforming XML documents into other formats. An XSL stylesheet
is a file containing transformation rules that define how to convert XML elements into different output formats like
HTML, text, or another XML structure.

#### XSLT Mediator

`eXtensible Stylesheet Language Transformations`

The XSLT Mediator takes XML input and transforms it according to rules defined in an XSL stylesheet. This enables
complex message transformations while maintaining the integration flow.
Transforms message payload based on an XSLT script. For faster XSLT transformation, use FastXSLT.

#### Configuration of XSLT Mediator

**`key`** is the key of the XSLT script stored in the registry.

Example Key: `conf:/xslt/transform.xslt`, where `conf` is the registry path, and `xslt/transform.xslt` is the file path.

**`property`**: Optional parameters to pass to the stylesheet

**`feature`**: Specify features to be enabled/disabled in the XSLT transformation.




#### Example

```xml

<xsl:stylesheet exclude-result-prefixes="m0 fn" version="2.0" xmlns:fn="http://www.w3.org/2005/02/xpath-functions"
                xmlns:m0="http://services.samples" xmlns:xsl="http://www.w3.org/1999/XSL/Transform">
    <xsl:output indent="yes" method="xml" omit-xml-declaration="yes"/>
    <xsl:template match="*">
        <xsl:element name="{local-name()}" namespace="http://services.samples">
            <xsl:copy-of select="attribute::*"/>
            <xsl:apply-templates/>
        </xsl:element>
    </xsl:template>
</xsl:stylesheet>
```

```
