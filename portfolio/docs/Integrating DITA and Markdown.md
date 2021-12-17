Darwin Information Typing Architecture (DITA) was first developed and used by IBM to standardize the company's documentation. Since 2001, DITA has become one of the most-used information formats in technical communication. DITA is useful for structuring content, especially in large businesses where information is often reused. DITA follows the single-sourcing method for managing content, where information is written in small chunks and then structured with extensible markup language (XML). XML organizes content using tags and data that are defined as topics written and combined to be used in a variety of contexts for multiple outputs.

Markdown was created in 2004 by John Gruber and Aaron Schwartz to be an easy markup language for the average person to use. It became popular among web writers and technical communicators because it made the process of formatting text quicker. It also works well in the world of web and app development. Markdown allows a writer to create headers, lists, word emphasis, and code blocks without lifting the hands from a keyboard. 

###DITA vs. Markdown
Technical communicators have sometimes disagreed about whether DITA or Markdown should be used for documentation. Critics of Markdown point out that the many "flavors" of Markdown that have developed means Markdown cannot be relied on as a standard for technical communicators. Those who use a particular flavor of Markdown will also find that it's more difficult to migrate a large set of Markdown documents to another tool that uses another markup language. 

Despite some misgivings, Markdown has continued to gain popularity because it is so useable and easy to learn. In the last few years, there has been more conversation among technical communicators about how to integrate Markdown with other tools that use more complicated markup language. Technical communicators who use both Markdown and DITA want to combine the strengths of both to complete documentation tasks. 

###The Backhoe and The Shovel
At the end of a [talk](https://www.youtube.com/watch?v=RNSvi2x1r-U) at the 2019 Soap! content conference, Patrick Bosek offered the following analogy to explain how technical communicators should think about DITA and Markdown:

>"Markdown is kind of like a shovel and DITA is like a backhoe. And you have these people who have never used a backhoe who are like 'that's way too complex. Why would you ever want to do that?' And then you have people who are construction workers who build big buildings and they're like--Why would you ever use a shovel? You can't build a big building with a shovel. If you're going to start a project by yourself and you don't know how to operate a backhoe, a shovel looks like the obvious answer. We've 
all used a shovel. But who in [this room] has ever used a backhoe. So they're just different. There's a place in the world for both of them and any construction site that's building something sufficiently large are going to have both of them there. And you don't have people arguing about whether or not we should eliminate shovels or backhoes."

>Patrick Bosek, (Living in Harmony: DITA and Markdown, soap! 2019 conference)

According to Bosek, DITA's strength is its longevity and stability. "DITA implementations oftentimes will last for decades," he says. "They will be installed and stay installed and producing value for ten or more years." On the other hand, "Markdown implementations can start in under a week." In other words, DITA is useful for well established companies that have accumulated a lot of information over the years. Markdown is helpful for startups or young companies that are trying to ramp up their productivity quickly. Markdown also fits better in an Agile environment where an iterative workflow takes the form of sprints, whereas DITA may be the optimal system for a marathon where the baton must be passed smoothly from year to year. Instead of arguing which system is best, technical communicators should consider how DITA and Markdown could work together to serve companies at various stages of development and according to particular work processes.

###How to Convert Markdown to DITA

Three information management specialists working at CISCO wrote a [blog post](https://www.infomanagementcenter.com/from-markdown-to-dita-and-back/) describing their experience moving Markdown files to DITA. One of the lessons they learned is to consider that Markdown files will inevitably have to be moved into DITA at a later stage of the information development process. At CISCO, technical communicators used a Git-Markdown process for collaboration. For an iterative process, this is preferable and could solve some of the issues technical communicators often find in a DITA environment where different contributors might have slightly different approaches to writing or structuring content within the company's information system. With DITA, these different approaches may not become apparent until later in the process. With GitHub, technical communicators and subject matter experts can work out an agreed-upon style or framework early on in the process, knowing that the changes they're making at that stage could make it easier to transition to DITA later on. 

There are many ways to convert Markdown files to XML so they can be used in a DITA information system. At the present time, this process requires more steps than many technical communicators would prefer. It appears that integration is an increasing priority for many companies, especially if software is a big part of their process or products, so it is likely we will see a more unified integration in the near future. 

[DITA Open Toolkit](https://www.dita-ot.org/dev/topics/markdown-input.html) (DITA-OT) currently allows a flavor of Markdown called [CommonMark](https://commonmark.org/) to be written directly in DITA topic references, and DITA content can be exported as Markdown too. With DITA-OT, a Markdown topic can be added to a DITA publication as long as the format is set to be attributed to Markdown:


```
<?xml version="1.0" encoding="utf-8"?>
<!DOCTYPE map PUBLIC "-//OASIS//DTD DITA Map//EN" "map.dtd">
<map>
    <topicref href="markdown-dita-topic.md" format="markdown"/>
</map>
```

When running DITA outputs (e.g. HTML or PDF), Markdown is temporarily converted to DITA but will remain a Markdown source file. This approach works best for simple content with multiple collaborators that has undergone lots of iterations before it's ready to be combined with more complex content in DITA XML.

###Conclusion
There are many methods and tools for integrating Markdown and DITA. In addition to DITA-OT, these include Lightweight DITA (LwDITA), pandoc,  Easy DITA, and the Oxygen batch converter plugin. For technical communicators, it's helpful to know the circumstances in which Markdown should be used, the most effective methods of iterative collaboration using Markdown and DITA, and the tools that make the migration of information between Markdown and DITA a smooth process.















