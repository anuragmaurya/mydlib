# mydlib
git: https://github.com/anuragmaurya/mydlib
Install using 'pip3 install mydlib'


Check test.py file for usage

    //test.py
    import mydlib 
    def test():
	#This is example for downloading single book from libgen.
    	print("starting simple downlad test")
    	book_name = "the road to reality"
    	mydlib.get_book_libgen(book_name)
    	print("book downloaded...")


	#for scanning your local library and saving it's information in catalogue 'catalogue_dir' 
    	directory = '../book_lib'
    	
    	catalogue_dir = 'catalogue_dir'
    	print("directory traversal catalogue test ...")
    	mydlib.create_catalogue(directory,catalogue_dir)
    	print("created catalogue by directory traversal...")

	#creating a library using catalogue file 'catalogue_dir'
    	print("starting to create library using catalogue file 'catalogue_dir'")
    	mydlib.create_library(catalogue_dir)
    	print("library creation completed")


	txt_file = 'txt_file.txt'
	#creating catalogue file using txt_file and saving to 'catalogue_txt'
    	catalogue_txt = 'catalogue_txt'
    	print("txt file reading catalogue test ...")
    	mydlib.create_catalogue(txt_file, catalogue_txt)
    	print("created catalogue by reading txt file")
    	print("starting to created library using catalogue file 'catalogue_txt'")
	
    	mydlib.create_library(catalogue_txt)
    	print("library creation completed")
    test()

Example txt_file 
//txt_file.txt

    books
    books/Project Tuva: Richard Feynman's Messenger Lecture Series - Microsoft Research.html
    books/Best Math Books - A Comprehensive Reading List. - Stumbling Robot core.html
    books/Advanced Topics. - Stumbling Robot.html
    books/All The Math Books You'll Ever Need | Math ∞ Blog.html
    books/Best Math Books - A Comprehensive Reading List. - Stumbling Robot.html
    books/Textbooks (Math and Statistics) - Mathematics - LibGuides at MIT Libraries.html
    books/Noam Nisan, Shimon Schocken - The Elements of Computing Systems_ Building a Modern Computer from First Principles-The MIT Press (2005).pdf
    books/Core Mathematics Subjects. - Stumbling Robot core.html
    books/MIT Department of Physics.html
    books/maths
    books/maths/Carl D. Meyer - Matrix analysis and applied linear algebra. With solutions to problems-SIAM_ Society for Industrial and Applied Mathematics (2001).pdf
    books/maths/pure mathematics
    books/maths/pure mathematics/tensor analysis
    books/maths/pure mathematics/tensor analysis/TensorsandtheirApplications.pdf
    books/maths/pure mathematics/tensor analysis/424b86d95a9e41a065629ab73773ee9e96b8.pdf
    books/maths/pure mathematics/tensor analysis/document.pdf
    books/maths/pure mathematics/combinatorics and graphs
    books/maths/pure mathematics/combinatorics and graphs/Combinatorics and Graph Theory.pdf


