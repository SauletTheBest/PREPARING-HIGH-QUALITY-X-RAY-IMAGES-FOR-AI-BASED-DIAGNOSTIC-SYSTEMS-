Appendix 3 — Interview transcripts 

Interview №1 

Date of Interview: 03.11.2025 
Time of Interview: 19.00-20.00 
Location: Online (Microsoft teams) 

Participants: Senior-lecturer on AITU Aldiyar Salkenov, reseacher, interviewer -Galymzhan  

As part of our research on “Preparing High-Quality X-Ray Images for AI-Based Diagnostic Systems,” we conducted an interview with a senior lecturer from the School of Software Engineering, who teaches the discipline Cloud Computing. The lecturer holds multiple academic degrees, including a Bachelor’s in Informatics (2015-2017) and a Master’s in Information Technology (2017-2020) from Gyeongsang National University, as well as a Bachelor’s in Automation and Control Systems (2013-2017) from Shakarim State University. 

His scientific interests include ICT4D, digital literacy, cloud computing, and machine learning, which align closely with the topic of our study. In addition, he teaches several relevant disciplines such as Web Technologies, Cloud Computing, Python, Operating Systems (Linux), and Research Methods and Tools. 

Given his expertise in machine learning and Python, this interview aimed to gain valuable insights into the technological and methodological aspects of enhancing X-ray image quality for AI-based diagnostic systems. Here are transcript of our interview: 

Galymzhan: 

How much does the quality of medical images (e.g. chest X-rays) affect the accuracy of machine learning models? 

Salkenov Aldiyar: 

Very strong. If the photo is blurry, noisy, or poorly lit, the model misses important details (like a shadow or a spot) and makes a misdiagnosis. The clearer and sharper the image, the more accurate the result! 

Galymzhan: 

What are the most common errors that occur when training models due to low image quality? 

Salkenov Aldiyar: 

For example, the model confuses healthy and diseased areas. Second, it doesn't recognize minor pathologies. It also produces too many false positives. It also doesn't generalize well to new images. 

Galymzhan: 

What normalization and filtering methods (e.g. CLAHE, Gaussian blur, rescaling) do you find most effective for medical images? 

Salkenov Aldiyar: 

CLACHE evens out contrast, making details visible. Gaussian Blur removes noise, but shouldn't be too strong. Rescaling makes all images the same size to avoid confusion! 

Galymzhan:  

How important is it to standardize all images (size, contrast, noise) before training neural networks? 

Salkenov Aldiyar:  

It's very important. If the images differ in size, contrast, or brightness, the model becomes disoriented. Standardization makes training stable and improves accuracy. 

Galymzhan:  

How do you evaluate the contribution of data quality to the final accuracy of deep learning models compared to the architecture of the model itself? 

Salkenov Aldiyar:  

Data quality is paramount. Even the best model won't help if it's trained on poor or unbalanced data. Good data = consistent results. 

Galymzhan: 

What Python libraries do you recommend for building preprocessing (e.g. OpenCV, NumPy, scikit-image)? 

Salkenov Aldiyar:  

There are many, such as OpenCV for filtering, resizing, and contrast. ScikitImage for advanced processing methods. And even NumPy for working with image arrays and matrices. 

 

Appendix 4 — Interview transcripts 

Interview №2 

Date of Interview: 02.11.2025 
Time of Interview: 22.00-23.00 
Location: Online (Zoom) 

Link:  https://youtu.be/6M19--HUiLc?si=5tUgGNaVq9xIPo2h  

Participants: Danil — Data Scientist, worker ML Specialist at Tinkoff Bank, currently CTO at two AI startups, Bekzhan — Researcher, interviewer 
 

We conducted an expert interview with Danil - a Data Scientist with over five years of professional experience in machine learning. Before transitioning into leadership positions in AI, Danil spent 2.5 years working at Tinkoff Bank, where he contributed to large-scale ML solutions. Earlier in his career, he worked as a Python developer, which provided him with a strong engineering background and a solid understanding of data processing pipelines. 

Currently, Danil serves as the CTO in two startups: one focused on matching founders with startups based on strategic and behavioral compatibility, and another building a platform for implementing AI tools in small and medium-sized businesses. His expertise in ML, data engineering, and Python development makes him highly relevant to the focus of our research. 

   

Bekzhan: 

How does the quality of chest X-ray images influence the accuracy of AI diagnostic systems? 

 

Danil: 

Image quality is one of the most important factors in machine learning. The accuracy of the final output depends directly on the quality of the input data. If the input is poor - noisy, blurry, overexposed, or lacking contrast - then no matter how good the model architecture is, the result will still be poor. In vision tasks this is especially critical: good input leads to good output. Poor data equals poor predictions. 

Bekzhan: 

- What common image problems (like noise or low contrast) most often reduce diagnostic accuracy? 

Danil: 

The most typical issues are noise, overexposure, underexposure, and low contrast. If an image is too dark, too bright, or noisy, the model struggles to identify key visual patterns. These distortions hide important features, making it much harder for the model to distinguish healthy tissue from pathological signs. As a result, diagnostic accuracy drops significantly. 

Bekzhan:  

Which preprocessing methods, in your opinion, are most effective for improving X-ray image quality? 

Danil: 

Primarily various filters: contrast-enhancing filters, brightness correction filters, and noise-removal filters. There are also additional algorithms that refine and normalize the image. Anything that increases contrast, reduces noise, or adjusts brightness helps bring the image to a format suitable for accurate model interpretation. 

Bekzhan: 

Do you think hospitals should follow a standardized image-preparation process before AI analysis? Why? 

Danil: 

Yes, absolutely. When a model is trained on one format and receives images in another, it may interpret them incorrectly or perform much worse. A unified standard ensures stability and prevents mismatches. While it’s technically possible to train a model to handle many formats and switch between processing branches, this is complicated and inefficient. It’s far easier and more reliable when all institutions follow a single format. 

Bekzhan: 

What can be done to make AI-based diagnostic systems more consistent and reliable across different hospitals? 

Danil: 

First, establishing a unified image format. Second, implementing a shared preprocessing pipeline that ensures all images are cleaned and enhanced the same way: removing overexposure, reducing noise, adjusting brightness, and improving contrast. This ensures consistent data quality across hospitals. Finally, regular testing is important - different tasks may require different preprocessing strategies, so evaluating multiple approaches helps find the most reliable solution for each scenario. 

 
