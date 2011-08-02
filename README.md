Python wrapper for the Bottlenose Wrapper for the Python Advertising Product API

Uses: bottlenose: https://github.com/dlo/bottlenose


Make a copy of local_settings.py.dist as local_settings.py and edit to fill in your AWS access and secret keys.


Example usage:


	from amazon import Search
	import webbrowser

	result = Search(title="The Idea of America",author="Gordon Wood",style="xml")	
	link = b.parsedXML['Item0']['URL']

	webbrowser.open(link)
