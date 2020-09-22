# Ever wondered "How Netflix manages to give us a best video and sound platform for streaming Unlimited movies, TV shows and more?"


![image](https://user-images.githubusercontent.com/61896468/93880426-1787fb80-fcfb-11ea-8396-96d0ccaab369.png)


## So, lets see how this all happens. Let's begin with this :

# What is Netflix? When did it come into existence? Some more about Netflix...

## Netflix, Inc. is an American technology and media services provider and production company headquartered in Los Gatos, California. Netflix was founded in 1997 by Reed Hastings and Marc Randolph in Scotts Valley, California. The company's primary business is its subscription-based streaming service which offers online streaming of a library of films and television series, including those produced in-house. As of April 2020, Netflix had over 193 million paid subscriptions worldwide, including 73 million in the United States. Today, the company produces and distributes content from countries all over the globe.


##  ` Netflix offers a wide variety of award-winning TV shows, movies, anime, documentaries and more – on thousands of internet-connected devices. You can watch as much as you want, whenever you want, without a single ad – all for one low monthly price. There's always something new to discover, and new TV shows and movies are added every week! Netflix has an extensive library of feature films, documentaries, TV shows, anime, award-winning Netflix originals, and more. Watch as much as you want, anytime you want.`


# How much does it cost?

## You can watch Netflix on your smartphone, tablet, Smart TV, laptop, or streaming device, all for one fixed monthly fee. Plans range from ₹ 199 to ₹ 799 a month. No extra costs, no contracts.

# Where can we watch Netflix?

## You can watch it anywhere, anytime, on an unlimited number of devices. Also, Sign in with your Netflix account to watch instantly on the web at netflix.com from your personal computer or on any internet-connected device that offers the Netflix app, including smart TVs, smartphones, tablets, streaming media players and game consoles. You can also download your favourite shows with the iOS, Android, or Windows 10 app. Use downloads to watch while you're on the go and without an internet connection. Take Netflix with you anywhere. Also, we can watch anywhere and cancel the subscription anytime.

![image](https://user-images.githubusercontent.com/61896468/93880684-79e0fc00-fcfb-11ea-866e-1bde0a397d66.png) 

![image](https://user-images.githubusercontent.com/61896468/93881280-51a5cd00-fcfc-11ea-8e1b-926f8f1b2f88.png)



# FACT: Netflix now has over 182 million subscribers (It's huge!!!!) worldwide. Isn't it too much ?

## So Now, there comes the most important question in our mind, which is :

# How does it manage to give service to their 182 million customers???

## This is because it outsources its entire technical or technological stuff. This includes using RAM, CPU, and many other resources like Electricity of Service Providers or Cloud Providers. These are called cloud computing companies. Netflix uses AWS - Amazon Web Services. Online content provider Netflix can support seamless global service by using Amazon Web Services (AWS). AWS enables Netflix to quickly deploy thousands of servers and terabytes of storage within minutes. Users can stream Netflix shows and movies from anywhere in the world, including on the web, on tablets, or on mobile devices such as iPhones. This is possible because AWS provides almost every domain service. Right now, Netflix is running more than 1 lakh+ Servers running at peak time on AWS. From this number, we can actually know how great is this.....


![image](https://user-images.githubusercontent.com/61896468/93880562-50c06b80-fcfb-11ea-9a77-c0f6ebf7d16a.png)

![image](https://user-images.githubusercontent.com/61896468/93881419-8023a800-fcfc-11ea-8e06-15cdc01d8e6c.png)

![image](https://user-images.githubusercontent.com/61896468/93881499-9e89a380-fcfc-11ea-95ad-31e2147bbff8.png)




# Netflix uses AWS for nearly all its computing and storage needs, including databases, analytics, recommendation engines, video transcoding, and more—hundreds of functions that in total use more than 100,000 server instances on AWS.

` Netflix has a fabulous team working on cloud and containers. Netflix started its migration towards AWS around in 2008 and it was a really long process. AWS brings highly scalable, elastic and secure cloud services to content production, storage, processing, and distribution. And with Machine Learning and Analytics embedded throughout the media value chain, you can make smarter content investments, better monetize your content library, and delight users with personalized experiences. 

 Microservice Architecture: Netflix while using AWS became more agile with the help of Decoupled applications and continuous deployment model. More agility resulted in faster innovation. Also, they built a diverse ecosystem of tools that included Spinnaker, Chaos engineering and Global cloud.
`

![image](https://user-images.githubusercontent.com/61896468/93880748-967d3400-fcfb-11ea-8eb8-f308b0d00f0c.png) 


# Blox and Working with AWS: Netflix wanted more control and so AWS listened. Blox includes:

## ECS integration with existing technology
## More roadmap definition
## Integrate Titus through Blox into ECS


![image](https://user-images.githubusercontent.com/61896468/93880841-b6acf300-fcfb-11ea-9894-9656a634ef85.png) 


## We will now have a look at how video is delivered to users by Netflix: It is through Open Connect. It is Netflix’s own Content Delivery Network (CDN) which it manages through Amazon. Videos that stream to a user are located in data centers within the networks of Internet service providers, facilities where traffic is exchanged among most of the network operators. The traffic is distributed directly to Verizon, AT&T, Comcast, and similar network operators at such exchange points. When a user presses ‘play’ button, from these sites, videos get delivered to him/her.

## Before a video gets delivered to him/her, operations like searching for videos and signing up by the user for the service are all handled in AWS cloud. Hence, the business logic, personalization, search, and data processing which gives the streaming experience are all live in AWS. The technology had to maintain Netflix’s employees who were working in streaming business, and this was also housed in Amazon.


##  `Now one more question that sparks our minds, that is : Do you know why Netflix took seven years to shift to Amazon? They rebuilt their entire software platform to leverage AWS cloud network to the maximum. ‘Chaos Monkey’ is a series of tools developed by Netflix to reduce damage in the case of disruptions. On the Christmas Eve of 2012, the company suffered a streaming failure and at the time it was on a single Amazon region. Since then, they have invested heavily in disaster recovery. Now, Netflix mainly operates in Oregon, Northern Virginia, and Dublin regions. What if one of these regions goes down? In this case, Netflix redirects the traffic to other available regions within a moment’s notice. The company has enough backups of all data which is stored in Amazon itself.`


# The distributed database, Cassandra is chosen to store customer data where every data element is replicated many times in production. The primary backups of all data are generated into S3 (Simple Storage Service). Any kind of operator errors, logical errors, software bugs, or other such corruptions can be dealt with by the S3 backups. ‘Armageddon Monkey’ is Netflix’s attempt to recover from failures of all its systems on AWS.

# The following is the architecture diagram:


![image](https://user-images.githubusercontent.com/61896468/93880933-d8a67580-fcfb-11ea-9885-adf3538e9e99.png) 





# Netflix Realizes Multi-Region Resiliency Using Amazon Route 53:

## What happens when you need to move 89 million viewers to a different AWS region? Netflix's infrastructure, built on AWS, makes it possible to be extremely resilient, even when the company is running services in many AWS Regions simultaneously. In this episode of This is My Architecture, Coburn Watson, director of performance and reliability engineering at Netflix, walks through the company's DNS architecture—built on Amazon Route 53 and augmented with Netflix's Zuul—that allows the team to evacuate an entire region in less than 40 minutes.

# `John Bennett who is a Senior Software Engineer at Netflix says - `


# "Amazon Kinesis Data Streams processes multiple terabytes of log data each day, yet events show up in our analytics in seconds. We can discover and respond to issues in real time, ensuring high availability and a great customer experience."

# Application Monitoring on a Massive Scale:

## Netflix uses Amazon Web Services (AWS) for nearly all its computing and storage needs, including databases, analytics, recommendation engines, video transcoding, and more—hundreds of functions that in total use more than 100,000 server instances on AWS.


## `This results in an extremely complex and dynamic networking environment where applications are constantly communicating inside AWS and across the Internet. Monitoring and optimizing its network is critical for Netflix to continue improving customer experience, increasing efficiency, and reducing costs. In particular, Netflix needed a solution for ingesting, augmenting, and analyzing the multiple terabytes of data its network generates daily in the form of virtual private cloud (VPC) flow logs. This would enable Netflix to identify performance-improvement opportunities, such as identifying apps that are communicating across regions and collocating them. The company would also be able to increase uptime by quickly detecting and mitigating application downtime.`


## Each log record carries information about the communications between two IP addresses. However, in a dynamic environment like the one at Netflix, where an IP address can float between applications from day to day or even minute to minute, IP addresses alone don’t have much meaning. “The data sources we had before we took on this initiative were one sided,” says John Bennett, senior software engineer at Netflix. “We’d know an application was connecting to others, but we didn’t know both sides of the conversation and how to optimize those communications or the placement of the applications on the network.”

## Netflix set out to establish a new data source that could give it more insight into communication among applications and regions by combining VPC flow logs with application metadata.

# Centralizing Flow Logs Using Amazon Kinesis Data Streams:


![image](https://user-images.githubusercontent.com/61896468/93881700-e14b7b80-fcfc-11ea-9909-f5b8061a9ea0.png)

![image](https://user-images.githubusercontent.com/61896468/93882010-3edfc800-fcfd-11ea-8e94-cd3174d49b06.png)



## From the outset, AWS enabled Netflix to experiment with different approaches to analyzing its network data. “Early in the design process, the flexibility to try different ways of processing the data was important,” says Bennett. “We experimented with multiple designs and used many AWS products to get here.”


## `The solution Netflix ultimately deployed—known internally as Dredge—centralizes flow logs using Amazon Kinesis Data Streams. The application reads the data from Amazon Kinesis Data Streams in real time and enriches IP addresses with application metadata to provide a full picture of the networking environment. “Usually, we would put the data into a database, which would build an index to enable faster querying,” says Bennett. “Dredge joins the flow logs with application metadata as it streams and indexes it without using a database, which eliminates a lot of the complexity.” `


##  The enriched data lands in an open-source analytics application called Druid. Netflix uses the OLAP querying functionality of Druid to quickly slice data into regions, availability zones, and time windows to visualize it and gain insight into how the network is behaving and performing.


## `AWS was the logical choice for Dredge in part because the data was already resident in the AWS Cloud. “It would have been daunting to publish, stream, and consume that much information from an external system such as Kafka,” says Bennett. “It took just a few API calls to centralize multiple terabytes of flow logs into Amazon Kinesis Data Streams. Now we can focus on getting insights from the data rather than simply getting access to it.” `

## `The scalability of Amazon Kinesis Data Streams was a good fit for the Dredge application because of the cyclical and elastic nature of network usage at Netflix.`




# Improving Customer Experience with Real-Time Network Monitoring

## Netflix’s Amazon Kinesis Data Streams-based solution has proven to be highly scalable, each day processing billions of traffic flows. Typically, about 1,000 Amazon Kinesis shards work in parallel to process the data stream. “Amazon Kinesis Data Streams processes multiple terabytes of log data each day, yet events show up in our analytics in seconds,” says Bennett. “We can discover and respond to issues in real time, ensuring high availability and a great customer experience.”

##  `Netflix is now able to identify new ways to optimize its applications, whether that means moving an application from one region to another or changing to a more appropriate network protocol for a specific type of traffic. “Our solution built on Amazon Kinesis enables us to identify ways to increase efficiency, reduce costs, and improve resiliency for the best customer experience,” says Bennett.`



## Although a streaming data solution is not new to the IT industry, it is an innovation in the networking space. “Netflix is heavily invested in AWS in part because it abstracts the underlying network, so we don’t have to deal with switches and routers,” says Bennett. “We’re monitoring, analyzing, and optimizing at a higher level of the stack—in ways we would never even consider if we were running our own data centers.”



# `Today, Netflix is the 10th largest Internet company in the world. Are you aware that during the peak traffic hours more than one-third of North American Internet traffic goes through Netflix’s systems? ‘Supporting such rapid growth would have been extremely difficult out of our own data centers; we simply could not have racked the servers fast enough,’ Netflix’s blog post says. It continues, ‘Elasticity of the cloud allows us to add thousands of virtual servers and petabytes of storage within minutes, making such an expansion possible.’ So, that is the power of Amazon Web Services propelling one of the most ambitious companies on earth, Netflix, into uncharted territory and runaway success! `

## Thus, AWS cloud provides Netflix a fully Reliable and Agile service being a service provider cloud computing company.




# And so the users of Netflix never ever face a delay of even 1 seconds.
