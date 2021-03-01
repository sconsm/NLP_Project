# Analyzing Children's Stories (NLP)
## *Why Is It So Important to Read to Our Kids?*
Metis NLP Project:
Using NLP to Analyze Children's Stories

### Introduction and Objectives:
At least **250 million** of the world’s 650 million primary school age children can’t read, write, or do basic mathematics! (According to United Nations 2014 findings). Not only is this number astounding, it's simply not ok. Reading is so important to young children's growth and development, however, not every child has the access to such resources. Thus, knowing how important reading is to children, my main question is: *why* is reading to our kids so important? I found it very interesting to look at language from the most basic reading level --at childhood. This is most likely everyone's first introduction to text language, so what can we learn from this. By exploring NLP techniques, I aim to understand what exactly is in the classic texts that children learn. What are the common themes in children's books? What can this tell us about how we shape our youth? Expanding beyond this projeect-- how can this knowledge of children's text help us provide all children with the necessary tools they need to grow. The overall objective of this project is to gain insights into the common themes within children's books. 


------

### Data Used:

Data gathered from the Gutenberg Project, a free online ebook website. 

https://www.gutenberg.org/ebooks/bookshelf/22?sort_order=downloads&start_index=26

There are 3 bookshelves related to children's books: **children's picture books, children's instructional books, and children's myths, fairy tales, etc.** I chose to create a dataset based on the top (most popular) books from each of the bookshelves. There are a total of 120 books in the dataset.


------

### Tools Used:
- pandas
- nltk
- numpy
- scipy
- sklearn
- matplotlib
- glob
- wordcloud

------

### Files Included:
Final Code: 
  - NLP_Final_Code.ipynb

Visualizations: 
  - Bar Graph of All Authors With Multiple Books.png
      - Visualization for Total Authors
  - Distribution of Topic Words for Topic 'Mystical Creatures'.png
      - Example of a chosen topic and the distribution of the corresponding topic words throughout all books
  - Distribution of Words Per Book.png
      - Graph of Words Distribution of all books
  - LDA Topic Model.png
      - Second type of topic modeling performed. Was the worst results.
  - NMF Model #1 (TfidfVectorizer).png
      - The best model from topic modeling. Gave the best topic results.
  - NMF Model #2 (CountVectorizer).png
      - Another form of NMF topic modeling, good results, similar to first model.
  - Wordcloud of Beatrix Potter's Book Titles.png
      - Displays only the titles of all of Potter's books. Gives a general idea of what her stories are about based on their titles
  - Wordcloud of T.W. Burgess's Book Titles.png
      - Displays only the titles of all of Burgess's books. Gives a general idea of what his stories are about based on their titles

------

### Possible Impacts and Practical Applications:
From the topic modeling of our data, we found the NMF model using TfidfVectorization provided the best overall topics for our data. These topics give us a generally good understanding of what chidlren's stories are about (based on this dataset). We can see how these stories, and the texts specifically, carry a lot of weight in children's understanding and development, and therefore are crucial for growth. These skills are carried on throughout young adult life, enabling children's abilities to think critically, and develop emotions like empathy. This project simply, emphasizes the need to really understand NLP in childrens stories!

#### Topics In Children's Books: Gutenberg Children's Books

Final Topics from NMF Modeling:

  - Nature and Outdoors
    - frog, pool, smiling, farmer
  - Animals
    - rabbit, garden, cat, mouse
  - Mythical Creatures
    - gods, giants, dragons, swords
  - Fairy Tales
    - knight, sword, lady, lord
  - Family and Relationships
    - papa, mama, aunt dear

------

### Future Work:
NLP has become very popular among early childhood development techniques, especially among parents. There are a lot of books and scholarly research articles on this subject matter that are very worth looking into. Overall, we have learned how important it is for childhood development for children to read and be read to, but unfortunately it is not something that many millions of young children have the privilege of receiving. This has many global limitations, and there is much more we can do to provide this basic human right to children everywhere. NLP could be used to help understand and solve global problems. If we understand how crucial text at beginner reader level is, we can use NLP to shape our children in the ways that we know they need in order to grow and develop to the best of their abilities.

Future work revolves around gethering more text data, expanding the types of books and working on a recommendation system that will help parents choose books for their children based on themes and topics they like. This encourages and promotes effective reading and engagement. The goal is to allow more children to be able to read and grow.

