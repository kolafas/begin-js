# Team Flash's Markdown task

## Music Genres
---------------
   Music can be simply put as an art or cultural activity that makes use of sound and silence. It obviously of course has its own categories which are reffered to as genres. A music genre is a conventional category that identifies some pieces of music as belonging to a shared tradition or set of conventions.
   There are basically three acceptable genres according to Musicologists which are as follows:
   
  1. [Art Music](https://en.wikipedia.org/Art_Music)
  2. [Popular Music](https://en.wikipedia.org/Popular_Music)
  3. [Traditional music](https://en.wikipedia.org/Traditional_Music)

# Entrepreneurship 
---
Enterpreneurship has traditionally been defined as the process of designing, launching and running a new
business, which typically begins as a small business, such as a startup company, offering a product, process or service for sale or hire.

## Accelerators that helps and teach people to start business
1. [Techstars](http://techstars.com)
2. [Ycombinator](http://ycombinator.com)
3. [500 Startups](http://500.co)


# OOP IN PYTHON

Unlike other most OOP languages, the pythonic way of implementing OOP principles is much more liberal and ‘wrongly so’ (according to many programmers with background in Java).
One of the popular deviations; the pythonic way to declare an attribute is to make it public unlike the general OOP principle of making attributes private and then creating setters and getters. In Python, the way is to make the attribute public and then using properties’ decorators, setting and getting the attributes are implemented.
Generally, python really does not have a private attribute; the implementation closer to it is the `self.__attribute` format which uses the [name mangling](https://en.wikipedia.org/wiki/Name_mangling) 'trick'.
~~~~
class oop_deviation:
	def __init__(self, value):
		self.data = value
	
	@property
    def data(self):
	    return self.__data
	    
    @data.setter
    def  data(self, data):
        if data < 0:
            self.__data = 0
        elif data > 1000:
            self.__data = 1000
        else:
            self.__data = data
~~~~

See [link](http://www.python-course.eu/python3_properties.php).