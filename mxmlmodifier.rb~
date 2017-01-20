require 'nokogiri'

filename = "output.docx/word/document.xml"
@doc = Nokogiri::XML(File.open(filename))
body = @doc.at_xpath("//*[local-name()='body']")
body.inner_html = ARGV[0]

File.write(filename, @doc.to_xml)


