Abstract—Real-time communication (RTC) is an important
part of modern convergence networks. The objective of our
project is to create a platform such that the user i.e a business
owner who tends to sell his/her product can start or create an
auction in which the interested buyers can join the environment
and by using real-time communication the auction is made
possible. This functionality helps the user to sell the product at
the best price possible when the user doesn’t know the market
value of the product. Also the buyer can add the review of the
product which will be converted into rating from 0 to 5.
Index Terms—real-time auction system, collaborative filtering,
recommendation model, sentiment analysis


To overcome the situation where a business owner doesn’t
know the actual value of the product in such a case the business
owner can use the proposed system to carry out an auction
in order to buy and sell online. The project tries to address
an issue that sellers face while selling used products online
by creating a real-time auction-based e-commerce website
that uses web socket programming in order to implement
this system. The system also uses a recommendation system
to recommend products to users according to their personal
preferences. Finally, the system also uses an NLP model for
sentiment analysis of comments on a seller’s profile.
A. Problem Description
To develop a real-time auction system that utilizes web
sockets for enabling real-time communication, Collaborative
filtering for recommending products to users and sentiment
analysis to analyze user comments and assign a rating to a
seller based on the reviews.
B. Problem Scope
The problem focuses on developing a real-time communication website that can host auctions in an effortless manner
allowing sellers to manage auctions and enabling them to sell
their items in a hassle-free way. It also aims at improving the
experience for the buyers by incorporating features such as
collaborative filtering based recommendation model for providing better product recommendations as well as a sentiment
analysis model that allows users to express their opinion in
form of reviews. These reviews are analyzed and based on it
seller receives a rating that is public.
II. IMPLEMENTATION DETAILS
The system is built in two sides: Server and Client side.
Server side has service and middleware, while the client side
is a real time website for auction. Website is a collection
of information pages that provided via Internet that can be
accessed around the world over the network connected to
the Internet. Client communicates to server through JSON
which act as a middleware of server. JSON (JavaScript Object
Notation) is a lightweight data interchange format, readable
and writable by humans, as well as easily translated and made
(generated) by the computer. The service has four services
which are node.js, socket.io, express.js, and mongo db. All
server – client data communication is communicated in both
ways.
Server’s services are using the Node.js with Express
framework, Socket.io and MongoDB, while Middleware are
using JSON. If the user uses a web-based chat application and
take action on the web, the web interacts with JSON JSON
then access the service, after getting the desired functionality
then JSON returns the results to the user.
Finally, the recommendation and sentiment analysis models
are served using Flask api. The models are designed and
trained using TensorFlow, a machine learning library for
python.
A. Architecture
Fig. 1. System Architecture.
B. Algorithms
1) Collaborative Filtering: Collaborative filtering is a recommendation technique that tries to identify patterns in the
preferences of a user in order to recommend relevant products
for that particular user. There are primarily two approaches of
implementing a collaborative filtering based recommendation
model.
• User-based collaborative filtering: This implementation
uses a user-item matrix in which each entry indicates
a level of preference for a given item by a particular
user to a particular item. This data is used to find similar
users with the help of similarity measures such as cosine
similarity, based on which recommendations are made to
the users.
• Item-based collaborative filtering: This approach uses
user-item interactions as its metric for calculating preference of a user for a particular item. Based on these
clusters of similar items are formed which are then used
for providing relevant recommendation to the user.
The proposed project uses a item-based collaborative filtering
approach for implementing a recommendation model. The
recommendation model consists of two phases. The first
phase is retrieval phase, it is responsible for retrieving the
relevant items from a given item set. The next phase is the
ranking phase in this phase the retrieved items are ranked
based on the preferences of the user.
2) Long Short Term Memory(LSTM): LSTM (Long ShortTerm Memory) is a type of recurrent neural network (RNN)
architecture designed to solve the problem of missing gradients in traditional RNNs. LSTMs are particularly useful for
sequential data processing, such as natural language text or
time series data.
The proposed project uses this LSTM model for sentiment
analysis on textual data. In the first stage, the input text is
preprocessed. Later this processed text is passed into LSTM
model. The model then returns the rating of that statement in
between 0 to 1. Later on the rating is mapped into the rating
between 0 to 5. The value near to 0 denoting the negative
review and the value closer to 5 denoting the positive review.
The average of all the values are taken to generate seller rating.
C. System Modules
AuctionIt is a platform where sellers are given an
opportunity to sell their products not only by mentioning
a initial price but by arranging an auction for the product
for the respective interested buyers, in which the buyers
will bid accordingly for the product and the buyer with the
highest and appropriate bid can buy the product. The focus
is on ”Web Real-Time Communication” through will live
communication for the auction can be smoothly carried out.
1) Seller: Sellers would be expected to log in every time
to view their profile, dashboard, add products to sell, schedule
and held auctions for respective product and etc. Sellers will
be able to add a new product which they want to sell, add
description about the product such as, image of the product,
features of the product, minimum amount at which the product
they want to sell.
2) Buyer: Buyers would be expected to log in everytime
to view the products available on the website at their home
page. The landing page of the buyer consists of the list
of products that are available for purchase, along with the
products the auction details are made available to the buyers
so in case they want to engage in buying the product, the
buyer can join the auction, bid accordingly, the bidding will
be respective to what other buyers are bidding. The buyers
can give reviews to the products and the reviews can be
further used for future references in buying other products.
D. Data Flow Diagrams
DFD-0:
Fig. 2. DFD-0.
Data Flow Diagram - 0 gives a high level overview of the
data interactions between different entities involved in the
system.
DFD-1:
Fig. 3. DFD-1
Data Flow Diagram - 1 gives a detailed representation of
the entire auction system.
III. RESULT
Fig. 4. Register Page
Fig. 5. Login Page
Fig. 6. Auction Page
Fig. 7. Home Page
Fig. 8. Post Ad Page
Fig. 9. Ad Review Section
Fig. 10. Feedback Section
Fig. 11. Purchase Section
IV. CONCLUSION
AuctionIt is a a real-time auction system that integrates a
collaborative filtering recommendation model and a sentiment
analysis model. By leveraging these models, the system offers
personalized item recommendations and sentiment insights,
thereby enhancing user experience and facilitating informed
decision-making.
V. ACKNOWLEDGMENT
We would like to acknowledge D. Y. Patil College of
Engineering, Akurdi for giving us this opportunity. We express
our gratitude towards all our faculty, project coordinator and
colleagues who have helped us directly or indirectly in completing this project, we were able to explore different aspects
of software development as well as research and for that we
are thankful..
VI. FUTURE SCOPE
The Auction website has a large area of expansion. One
area is to add a private auction in which the seller can invite
only a specific number of people via a special link.
