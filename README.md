# HTML/Web Media Scraper
[Try it out on Apify](https://apify.com/aweworkz/html-web-media-scraper)



### Overview

The Web Media Scraping Tool is a powerful utility designed to extract various media files, including images, videos, audio, and other related elements, from multiple websites. It provides a convenient way to gather media content and retrieve associated descriptions or alt="" content. The tool supports output formats such as JSON or CSV and offers proxy support for websites with bot blocking features.

  

This documentation provides a comprehensive guide to the Web Media Scraper, a powerful tool designed to automate the process of collecting media files (images, videos, audio) and their corresponding descriptions from various websites.

  

### Features

- Automated Extraction: Saves time by automatically collecting media from multiple websites.

- Rich Media Support: Captures images, videos, audio, and other relevant media elements.

- Description Retrieval: Extracts associated descriptions like "alt" text for accessibility.

- Flexible Output Formats: Choose your preferred format for seamless integration - JSON or CSV.

- Optional Proxy Support: Overcome website bot-blocking measures if necessary.

  

### Benefits

- Increased Efficiency: Effortlessly gather media and descriptions from numerous websites in one go.

- Time-Saving: Automate the data gathering process, freeing your time for analysis and creative work.

- Streamlined Workflows: Easily integrate extracted media and descriptions into your projects.

  

### Common Use Cases


Content Curation and Aggregation:

- Use the scraper to aggregate images from multiple sources, facilitating content curation for blogs, social media posts, or marketing campaigns.

Market Research and Competitor Analysis:

- Analyze images used by competitors or within specific industries to gain insights into market trends, preferences, and branding strategies.

Brand Monitoring and Reputation Management:

- Monitor image usage across various platforms to safeguard brand integrity and address any unauthorized or detrimental use of brand assets.

Identifying Influencer Partnerships:

- Identify potential influencers or content creators by tracking the images they share, enabling strategic partnerships for brand promotion.

Product and Image Recognition:

- Train machine learning models using scraped images for tasks like product recognition, visual search, or image classification.

Research and Data Analysis:

- Collect images for research purposes, such as studying visual trends, analyzing user-generated content, or conducting sentiment analysis.

Content Personalization:

- Utilize scraped images to personalize user experiences on websites, apps, or marketing materials based on user preferences and behaviors.

Digital Rights Management:

- Monitor image usage to enforce copyright protection, identify instances of infringement, and ensure compliance with intellectual property laws.

E-commerce Optimization:

- Extract product images from e-commerce platforms to analyze pricing strategies, competitor offerings, and visual merchandising tactics.

Event Tracking and Reporting:

- Capture images related to specific events, campaigns, or product launches for comprehensive tracking and post-event analysis.

  

### Input
The actor requires only the website URLs from which to retrieve images and information on which proxies to utilize. You can specify multiple websites to obtain multiple results in a single run.
```json 
{
   "startUrls": [
       {
        "url": "https://apify.com",
       },
   ]
}
```

### Output
The actor saves its outcomes in the default dataset linked with the actor's operation. Subsequently, it offers the flexibility to export the data into different formats, including JSON, XML, CSV, or Excel.

Each website within the dataset is represented as a distinct object following this structure (illustrated in JSON format below):

```json
[{
  "URL": "https://crawlee.dev/docs/guides/configuration",
  "total_media": 5,
  "media_elements": [],
  "images": [
    {
      "id": "s6OotqTrMLa",
      "url": "https://crawlee.dev/docs/guides/configuration",
      "src": "/img/crawlee-light.svg",
      "alt": "",
      "type": "image"
    },
   
    {
      "id": "ZESUvm5A47e",
      "src": "/img/crawlee-dark.svg",
      "alt": "",
      "url": "https://crawlee.dev/docs/guides/configuration",
      "type": "image"
    }
  ],
  
   "svg": [
    {
      "id": "JwdyTS8P6Kt",
      "url": "https://crawlee.dev/docs/guides/configuration",
      "type": "svg"
    },
    
    {
      "id": "0r4WQSDIyNV",
      "url": "https://crawlee.dev/docs/guides/configuration",
      "type": "svg",
    }
  ],
  "videos": [],
  "audios": [],
  "embed": [],
  "object": [],
  "canvas": [],
},

```

**Important:** If you require customization or wish to request additional features, please feel free to contact us via <a href="mailto:holymark0001@gmail.com">email   </a>. We aim to respond to all inquiries within one business day, ensuring prompt assistance and addressing your needs effectively.
