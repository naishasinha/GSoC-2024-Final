<div align="center">
  
# Google Summer of Code 2024: Final Project

***

<img width="1381" alt="Screenshot 2024-06-07 at 12 36 29 AM" src="https://github.com/naishasinha/GoogleSummerOfCode2024-FinalReport/assets/117387359/f6fc2919-725b-4339-9a49-30f8c2f5391b">

***
  
| Contributing Software Developer: | Naisha Sinha|
| ------------- | ------------- |
| **Project**:  | [Automating Quantifying the Commons](https://summerofcode.withgoogle.com/programs/2024/projects/vvuGqMLQ)  |
| **Organization**:  | Creative Commons  |
| **Mentors:**  | <table><tr><td>**Lead**:</td><td>Timid Robot Zehta</td></tr><tr><td>**Supporting**:</td><td>Shafiya Heena, Sara Lovell</td></tr></table> |

***

## Project Description

### • Context and Problem •
<div align="justify">
  
[Quantifying the Commons](https://github.com/creativecommons/quantifying), an initiative emerging from the UC Berkeley Data Science Discovery Program, aims to quantify the frequency of open domain and CC license usage for future accessibility and analysis purposes. Till date, the scope of previous project advancements have not included automation or combined reporting, which is necessary to minimize the potential for human error and allow for more timely updates, especially for a project engaging with substantial streams of data.
</div>

### • Primary Objective •
<div align="justify">
  
The overarching goal of this project is to develop automation software for data gathering, flow, and report generation, ensuring that open-domain and license reports are never more than 3 months out-of-date.
</div>

### • Overall Impact •
<div align="justify">
  
With over 2.5 billion licenses globally, Creative Commons has become integral to the digital landscape, facilitating the sharing and utilization of creative works across diverse domains. Therefore, the impact of this initiative extends beyond streamlined processes; it promises to empower researchers, policymakers, and stakeholders with up-to-date insights into the global usage patterns of open domain and CC licensed content. By setting a precedent for effective data-driven initiatives, Quantifying the Commons and its related undertakings, including this one, pave the way for future advancements in comprehending and leveraging open content licenses worldwide.
</div>

***

## Contributions and Accomplishments

<div align="left">
  
(1) All of the comprehensive code contributions can be accessed within this pull request: [CC Quantifying PR #123](https://github.com/creativecommons/quantifying/pull/123). In total, I was responsible for 7,617
net code additions across 128 commits and 61 files. <br> <br>
(2) In addition, I've developed an in-depth [documentation page](https://unmarred-gym-686.notion.site/Automating-Quantifying-the-Commons-Documentation-441056ae02364d8a9a51d5e820401db5) for this project, either for those interested in learning and using the software, or developers who will be building upon the code in the future. <br> <br>
(3) For a more detailed perspective on the entire development process, please refer to my blog posts ([Part 1](https://opensource.creativecommons.org/blog/entries/2024-07-10-automating-quantifying/) and [Part 2]()) on CC's technical blog page. <br>

</div>

### • Completed Deliverables Over the Summer Period •

| Deliverable | Description|
| ------------- | ------------- |
| Phase 1: Fetch Data  | Building on previous efforts in the Quantifying initiative, this phase efficiently fetches raw data from various data sources using APIs. The retrieved data is then stored in a structured CSV format, preparing it for processing and analysis. |
| Phase 2: Process Data (Outline)  | This phase focuses on analyzing the fetched data between quarters. Since only `2024Q3` data (07/01/2024	- 09/30/2024) could comprehensively be generated during the summer period, a psuedocode outline of analysis was developed. Although this phase will be further solidified as more quarters and years pass by, a base error system was tested and implemented during the GSoC period to ensure thoroughness for this phase. |
| Phase 3: Generate Reports  | The final phase successfuly creates visualizations and reports based on the generated datasets. These reports are designed to present key findings and trends in a clear, concise manner, and have been designed to automatically be integrated into a quarterly README file to provide a comprehensive overview of license data across data sources. |
| Shared Module | Created a singular, shared module to organize and streamline the codebase, allowing different directories, paths, and components to be imported through that module across different files.|
| Directory Sequence (OS) | Using Operating System (OS) Modules, the codebase effectively facilitates the interaction between all three phases, ensuring smooth communication of 10 different data sources with their respective data storages.|
| Automation using GitHub Actions CI/CD | All three phases of the project — data fetching, processing, and reporting — have been automated using YAML scripts in GitHub Actions. This CI/CD pipeline ensures that every update to the codebase triggers the entire workflow, from data retrieval to the generation of final reports, maintaining consistency and reliability across the process. Cron functions are used to ensure that these scripts are run every quarter in a timely manner. |
| Custom Error and Exception Handling System | Implemented a custom exception system that centralizes the error-handling logic, keeping the codebases more specific, maintainable, and consistent overall. This system has been thoroughly tested and verified across all three phases. |
| Project Directory Tree | Added a structured layout of the project (hierarchical representation of directories and files with descriptive comments), which provides developers with a clear understanding of the project's organization and help them navigate through different components easily. |
| Data Flow Diagram (System) | Finalized an overall data flow diagram to establish an official framework for the codebase's system design.|
| Comprehensive Documentation | This document was developed to serve as a reference guide for any contributors having questions or needing detailed clarification on specific topics within the Quantifying codebase — each section has its own page with expanded information. It also includes external references and documentation regarding the languages and tools used for this project. |

### • Flow of System and Data •
`1-fetch` `2-process` `3-report`


<img width="70%" alt="Final DFD" src="https://github.com/user-attachments/assets/df329fb0-4ebe-494e-b308-ba84c03b676d">


### • Comprehensive Technologies and Tools •
Incoming

***

## Final Conclusions, Acknowledgments, Next Steps

### • Overall Growth + Limitations + Gratitude •
<div align="justify">
  
Although this 12-week period provided a vast amount of time to grow the Quantifying codebase, there were still time and resource constraints that we had to consider; primarily, the lack of data we could collect using the given APIs over this time period. However, as mentioned earlier, given strategic implementations, I was able to still complete the summer goal of developing a baseline automation software for data gathering, flow, and report generation, ensuring script runs on a quarterly basis. 

Working on this project individually has pushed the boundaries of my skillset and expertise to heights that I had never knew would be possible in such a limited amount of time. Going into this venture, I only had basic experience within full-stack development principles. Upon completion, however, I left with an augmented comprehension of utilizing modular operating systems, strategizing edge-cases and error handling for large data streams, programmatically interacting with software workflows within CI/CD pipelines, and much more. 

The completion of this project would not have been possible without the constant guidance and insights of my mentor(s). It is remarkable how easily they created a safe
space for an emerging developer since the very beginning, allowing me to feel open to ask questions and explore new side initiatives that facilitated my growth. The fast
progress and depth of my deliverables was solely due to the vast techical experience that they constantly shared with me.
</div>

### • Next Steps •
incoming

***

</div>
