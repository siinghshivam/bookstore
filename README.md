#class book store
#Add a book
#remove a book
#count a book

class bookstore():
  counter = 0
  def __init__ (self):   
   self.books =[]


  def add(self,book):
    if book not in self.books:
      self.books.append(book)
      bookstore.counter += 1
    else:
        print("We already have "+ book +".")

       
  def delete(self, book):
    if book in self.books:
      self.books.remove(book)
      bookstore.counter -= 1

    else:
              print("No such book")            

  def show_all(self):
     print(self.books)

my_bookstore = bookstore() 
my_bookstore.add('sara')
my_bookstore.add('Ashutosh')
my_bookstore.add('Shivam')
my_bookstore.add('avinash')

my_bookstore.delete('Aiyappa')
my_bookstore.delete('sara')
print(bookstore.counter)

my_bookstore.show_all()

 
 
 # we have created a book store added certain books in that and intitated the counter as well to track the no of books 
 and when we will remove any book it will remove existing books and count also decrease.
 # in adding book we have done the same if any will try to add existing book it will show book already exist and if not preset book will added and it willincrease the counter as well.
