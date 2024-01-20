# Data-Mesh
What is data mesh?
Imagine your company's data practices like a well-organized party. A cool thing called data mesh can make sure everyone at the party can easily access and use important information. It helps your data setup grow and work better, getting rid of messy connections in your data systems.
This data mesh thing is influenced by cool concepts like microservices, data fabric, data marts, event streaming, and domain-driven design. There are four main ideas behind data mesh: each section owns its data, data is treated like a valuable product, there's a platform for easily getting data, and there's a big plan for how everything is managed together.

Domain Ownership Principle: This one says that teams should be in charge of their own data. Instead of one big team managing all the data, each group should handle the data related to their specific area. It's like organizing data based on what each team is responsible for.
Data as a Product Principle: Think of data like it's a product that different teams can use. The team that owns the data should make sure it's good quality and useful for others. It's like treating data as something everyone can access and use, just like any other tool.
Self-Serve Data Infrastructure Platform: This means having a special team that provides tools and systems for all the different teams to work with data easily. They create a platform that makes it simple for everyone to use and create data products without too much hassle.
Federated Governance Principle: This one is about making sure all the data products work well together. There's a group that sets the rules and standards so that everything is organized and follows the company's and industry's guidelines.


Data Mesh Architecture 
 

So, there's this thing called "data mesh architecture," which is like a cool way of organizing information. Imagine you have different teams, and each team is like its own little world called a "domain." Each team is responsible for its own data – both the day-to-day stuff and the more in-depth analysis.

Here's the cool part: each team can analyze their data all by themselves! They take the everyday data, do some smart stuff to make it easier to understand (we call this "analytical data models"), and then use it to figure things out. And get this – if they want, they can share these smart data things with other teams.

Now, to make sure everyone is on the same page, the teams agree on some big rules together. This includes how different data pieces can work together, making sure everything is safe, and having clear instructions for everyone to understand (like a rulebook). This group that sets the rules is called the "federated governance group."

To help the teams work better with their data, there's a special team called the "data platform team." They create tools that any team can use, making it super easy to understand and work with data. And there's another helpful team that guides everyone on how to use these tools and make sure their data works well with others.

So, data mesh is like a teamwork approach to data – each group manages its own info, shares if they want, follows some big rules, and uses tools to make everything run smoothly. 
Elements.
Data Product
Imagine a data product like a super organized box of information that a team can use for analyzing data. It's like a smart module or microservice, but for looking at data in-depth. Teams connect data products to different sources, like systems or other data products, and then transform the data into something understandable. The data can be shared with other teams through something called "output ports," which are like structured datasets. 

Each data product belongs to a team, and that team is responsible for it from start to finish. They have to make sure the data is good quality, always available, and not too expensive. To design these data products, teams can use something called the "Data Product Canvas." And to keep track of them and make sure everything is in line, there's a tool called "Data Mesh Manager."

Data Contract
Now, think of a data contract like a set of rules for exchanging data between teams. It's like an agreement that says how the data should be structured, used, and what to expect. It covers things like who provides the data, how it can be used, what it looks like, and even billing details. This contract is crucial when different teams share data. It helps everyone understand and use the data properly.

Federated Governance
Next up, we have the "federated governance group." This group is like a team of representatives from all the groups in the data mesh. They make global rules, like how the different teams should build their data products. These rules ensure that everyone can use the data products in a similar way. For example, they might decide that all data should be provided in a standard way, like a CSV file on AWS S3.

Transformations
Now, let's talk about how data changes within a data product. Operational data, which is like raw and unstructured info, gets cleaned and structured into events and entities. Events are like small, unchangeable bits of info, and entities represent things like shipments or articles that change over time. Teams also integrate data from other teams, combine it to answer questions, and can publish it to other teams using data contracts.

Ingesting
How do teams get their operational data into the data platform? Well, they use something called domain-driven design, where they treat data as mutable entities and immutable domain events. These events are like business facts, and teams can forward them to the data platform in real time. There are different tools, like Kafka Connect and AWS Lambda, that help with this.

Clean Data
Clean data is super important for good analytics. Each team is responsible for cleaning their own data because they know their domain best. They take the raw, messy data and structure it, fix any issues, and make sure it's complete and accurate. There are different ways to do this, like using SQL views or even more advanced tools like Apache Beam.

Analytics
Now, how do teams gain insights from their data? They use SQL for most queries and powerful functions to connect and investigate data. Notebooks help to explore findings, and there are cool visualization tools to make data easy to understand. For advanced insights, teams might use data science and machine learning methods, but these require some special skills.

Data Platform
Lastly, we have the data platform, which is like the playground where all the data action happens. It can vary for each organization, but it helps teams build and run analytical models and access data products. There are analytical capabilities that help with data analysis and data product capabilities for creating, monitoring, discovering, and accessing data products. The platform also supports policies to make sure everything follows the rules without manual work.

Demo:
Inside the demo environment with an e-commerce: 
we can create our own data mapping , there’s a free trial demo without registration, within the headers tab, we have options to choose within for owner and status section with also (Data Products , Source system ,domain teams, adding extra data product which the terms are mentioned above )
Data Mesh Manager: This is a tool or platform designed to help manage and govern data within a Data Mesh architecture. It likely provides functionalities related to discovering data contracts, tracking data products, managing policies, and ensuring compliance within a decentralized data ecosystem.
Demo Environment: The environment you are entering is a demonstration or simulation. It's not a live production system but rather a place where you can experiment and get a feel for how the Data Mesh Manager works.
E-commerce Example: The demonstration uses an e-commerce scenario. This suggests that the data being managed and analyzed might be related to an online store. For example, you might find data contracts for orders, which could include information about customers, products, and transactions.
Data Contract for Orders with PII: The message specifically mentions exploring a data contract for orders that includes Personally Identifiable Information (PII). This points to the idea that within this demo, you can check how data contracts define and handle sensitive information like customer details within the context of e-commerce orders.
 
