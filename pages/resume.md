- PDF version: ![Anuraj Pandey Resume.pdf](../assets/Anuraj_Pandey_Resume_1727903809364_0.pdf)
- Contact
  collapsed:: true
	- **[LinkedIn](https://www.linkedin.com/in/anuraj-pandey-5749b48/)**
	- San Francisco, CA
	- anurajpandey11@gmail.com
- Work experience
  collapsed:: true
	- Director AI Engineering, Blueshift Labs, San Francisco (June 2016 - Current)
		- Roles
			- Director of Engineering, AI (Jan 2020 - Current)
			- Engineering Lead, AI (June 2016 - Aug 2018)
		- Responsibilities
			- collapsed:: true
			  
			  AI Product Engineering - AI studios, assistants and analytics
				- Built AI studios ([recommendations](https://blueshift.com/content-product-recommendation/),[predictive audiences](https://blueshift.com/predictive-audiences/),[insights](https://blueshift.com/customer-insights/)) for growth marketing teams to automate and personalize customer engagement with content recommendations, predictive scores and conversion optimization
				- Built [CDP assistants](https://blueshift.com/generative-content/) and evals for customer personas discovery and personalized content messaging using finetuned LLMs
				- Built real-time analytics and attribution infra/services, which power[AI decision-making for customer journeys](https://blueshift.com/channel-time-intelligence/) using[send time and channel optimization](https://blueshift.com/blog/send-the-right-message-at-the-right-time-with-engage-time-optimization/) and auto winner selection algorithms
			- ML Modeling - retrieval, recommendations, LLMs, predictive scoring
			  collapsed:: true
				- Large scale vectorization of user, catalog interactions using deep learning architectures to build retrieval and ranking models
				- Built AutoML propensity models for [next best actions](https://help.blueshift.com/hc/en-us/articles/360025114414-Set-up-predictive-models), scoring 100M+ customer profiles per day
				- Sequence prediction modeling for multi-dimensional event sequence data with transformers architectures and custom tokenizers to automate feature engineering
				- *Tech - pySpark, scikit, pyTorch, autoencoders, H2O.ai, mllib, ALS, KNNs, faiss, xgboost*
			- collapsed:: true
			  
			  ML Infra - inference, feature stores, mlops, obervability
				- Designed [real-time personalization service](https://blueshift.com/blog/blueshift-recommendations-studio-recipes-rank/) in rust fetching and ranking 1000s of candidate items with p95 latency of 100ms, serving billions of 1-1 personalized recommendations a month
				- Developed spark based feature engineering framework for graph sequence data (user x catalog x events) to serve offline/online feature/embedding stores with builtin time travel, backfills, feature observability
				- Built a centralized MLOps framework which streamlines deployment and lifecycle management of ML jobs by unifying scripting, configuration management, feature flags, versioning, instrumentation, logging, dependency management, containerization, providing complete observability around SLA management
				- *Tech: Scylladb, Rust, Ruby on Rails, Python, Nomad, pyspark, Consul, Terraform, MySQL, Redis, Datadog, Airflow, ONNX*
			- Data Infra - lakehouse, ETL, distributed systems
			  collapsed:: true
				- Realtime ingestion and organization of billions of customer profile and engagement events into 1000s of feature stores served by Hbase, Scylladb and deltalake features tables with a few mins/hours latency
				- Operational ownership and management of 10,000+ batch ETL hive/spark jobs processing TBs of data catalogs per day on a 5000+ vCores YARN cluster
				- Deployed a 500+ vcores[Druid cluster serving realtime dashboard analytics](https://imply.io/blog/blueshift-scaling-real-time-campaign-analytics-apache-druid/) on 100s of billions of datapoints
				- Deployment of large airflow and nomad cluster fine tuned to run 100k+ jobs a month across 100s of DAGs
				- Improved 30% data infra cost, 3% operating margins, 60% application performance through modernization of data/ML infra stack, managed autoscaling of spark jobs and migration of on-prem hadoop to AWS EMR
				- *Tech: Spark, HBase/Hudi/DeltaLake, Hive/Glue, S3/HDFS, Parquet/ORC, AWS EMR, Kafka/Pulsar *
		- Leadership
			- Career management, product, customer success
				- Built a cross functional AI/ML Engineering team from scratch, managing product strategy, engineering R&D roadmap, career management of 8 direct reports
				- Customer success and AI solutions onboarding and deployment in retail, media, personal finance, [AI in Marketing course](https://academy.blueshift.com/p/becoming-an-ai-marketer), contributions to AI ROI benchmark reports and whitepapers for demand generation
	- Senior Software Engineer, Optimizely, San Francisco (Aug 2014 - June 2016)
		- Built a low latency behavioral targeting service, high throughput realtime data ingestion pipelines, customer profile store, sdks to extend optimizely’s client side audience targeting with cross channel server side targeting
	- Senior Software Engineer, Amazon, Bangalore (June 2011 - June 2014)
		- Automation of new item setup audit workflow using rule based micro services and NLP intelligence, auto auditing 75% of new products across 3 product lines with 99.3% accuracy
		-
		-
- Education
  collapsed:: true
	- IIIT Hyderabad 2007-2011
		- B Tech (GPA: 8.17)
- Skills
  collapsed:: true
	- Data - hadoop, hive, spark, hbase, pyspark, druid, mysql, redis, memcache, parquet;
	- Languages - python, ruby, scala, java, c++, javascript;
	- ML - scikit, mllib, H2O, pandas, fastai, pytorch, recommenders system, AutoML, propensity modeling, auto-encoders, collaborative filtering, NLP embeddings , Faiss;
	- Ops - chef, terraform, nomad, consul, datadog, rollbar, opsgenie, prometheus;
	- AWS Cloud - ECS, EC2, EMR, S3, cloudwatch, cost explorer, glue, sagemaker, bedrock, Q, SQS, lambda, athena; GenAI - cursor, claude, bedrock, chatgpt