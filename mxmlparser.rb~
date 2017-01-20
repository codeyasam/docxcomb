require 'nokogiri'

@doc = Nokogiri::XML(File.open(ARGV[0]))
bodyContent = @doc.xpath("//*[local-name()='body']").inner_html	
print bodyContent
