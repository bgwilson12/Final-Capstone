# Final-Capstone
The final capstone project for the Thinkful Data Science Bootcamp

Here is my project proposal, I think it sums everything up pretty nicely so I'll just post it here.

## Final Project Proposal
The following is my final capstone project proposal for the review of the Thinkful Staff. I have included the prompts given in the assignment and will answer each of them individually.


#### What is the problem you are attempting to solve?
There are hundreds of websites called "Essay Mills" that offer a variety of services to students. Some of these services include:
- Shopping for a pre-written essay (purchasing it means they will take the essay down from their services in order to fool anti-plagiarism services).
- Paying a proffessional author to write an original essay (sometimes not original, depending on how sketchy the site is)
- Paying to have a pre-written essay rewritten, just for you, in order to fool anti-plagiarism services.

The services are technically legal, though most schools consider this to be academic dishonest (cheating) and take action against the students that use them. Anti-plagiarism services are unable to detect these papers because they are in fact original. Students that pay to cheat on papers not only put their classmates at a disadvantage, they are also damaging the reputation of the university by being dishonest and lazy. 



#### How is your solution valuable?
The anti-plagiarism site [Turn It In](turnitin.com) works by comparing a student's work to thousands of other works. With each submission, their database of original works grows. Essay sites are a huge pain for universities, because as long as the site is actually writing original content for students, they are able to fool anti-plagiarism services such as Turn-It-In. An essay mill detection service does not currently exist, and if combined with an anti-plagiarism service's resources, could be quite powerful.



#### What is your data source and how will you access it?
My data source is https://www.ukessays.com/essays/philosophy/ (for now, I will need more) and I will be using a Scrapy spider. I was going to break the student essays into chunks that were roughly equal to the size of the professional samples, and vice-versa. In addition, I want to cluster the essays in such that I could throw out clusters that consist only of student samples, if needed. I would do some research into how often students use these sites in order to figure out the proper ratio of student samples to professional samples.




#### What techniques from the course do you anticipate using?
I will use cross-validation with a training/validation set, and I will use a test set for final evaluation. More than likely, I will have to do a lot of web-scraping using a Scrapy Spider, followed by extensive pre-processing and cleaning of the data using matplotlib and pandas. I anticipate using most of the sklearn classification algorithms, and evaluating them with f1 and AOC metrics. In addition to using SVD for dimensionality reduction, I will try Sense2Vec and clustering algortihms that can select their own clusters.



#### What do you anticipate to be the biggest challenge you’ll face?
I think finding enough data could prove difficult. Learning to use Scrapy might be tough as well. I feel very confident in my ability to process/analyze large volumes of text, given my previous project experiences, as well as building the algorithms themselves. If I decide to use Sense2Vec, I may run into difficulties there. I attempted to use Doc2Vec on my supervised capstone, only to get poor results. I did not realize at the time that the use case for Doc2Vec was slightly different than what I was attempting to do, so hopefully the experience gained there will help me.
