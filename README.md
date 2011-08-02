Python wrapper for the Bottlenose Wrapper for the Amazon Product Advertising API

Uses: bottlenose: https://github.com/dlo/bottlenose


This is a sort of specialized wrapper for a wrapper (I realize the redundancy) that focuses on automated uses like showing product results in python generated content or simply using as a terminal-based Amazon search tool, as demonstrated below. It is still a work in progress and is evolving as it meets the need of a collaborative project in which we are integrating this functionality. So please bare with me as things get tweaked and focused.


To start:

	Make a copy of local_settings.py.dist as local_settings.py and edit to fill in your AWS access and secret keys.


Example usage:


	from amazon import Search
	import webbrowser

	result = Search(title="The Idea of America",author="Gordon Wood",style="xml")	
	link = b.parsedXML[0]['URL']

	webbrowser.open(link)
