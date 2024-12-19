- 👋 Hi, I’m Wesley Lee a.k.a @molonfac
- test website is https://main.d3osgv73xfwcfl.amplifyapp.com on AWS Amplify
- AWS Amplify was chosen as it is by far the easiest to create and host a simple website and has some level of protection such as firewall features and IP/geolocation restrictions. It also comes with super simple CI/CD build and built-in monitoring page, which is a plus for its familiarity 
- If I had more time, I would:
  - Set up Route53 record on hosted zone, with Cloudflare registered then have it coupled with Amplify custom domain. Cloudflare has good level of analysis on the activities on the domain. Also the URL will not be ugly
  - Set up this repo to connect with Amplify, so S3 bucket to hold the index.html file won't be needed - I had trouble setting up Amplify application access to this repo, so unfortunately I could not do it.
- Alternatively ECS, EC2 or S3 static site were considered however:
  - ECS and EC2 has too much overhead for the other resources to make it happen, such as VPC, Security groups, its rules, IAM roles, loadbalancer and route53 records just to make it accessible.
  - S3 static site could be good and simple but Amplify lets me even skip all of that.
- Production grade website will require at minimum:
  - a repository to host its code in order for developers can work to improve and maintain its functionality
  - CI/CD pipeline to ensure build/test/publish steps are streamlined
  - depends on the company's engineering practices, a separate repo or standardized infrastructure portions of the code snippets which manages the resources to be created in the platform (Cloud or on-prem)
  - Cloudfront if the infrastructure is in AWS, will be one of the good choice to increase the availibility and accessibility of the website. Although personally prefer Cloudflare for the distribution and the security features that comes with it.

<!---
molonfac/molonfac is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
