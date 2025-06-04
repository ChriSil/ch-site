+++
# Standard Zola front matter (you can add more like 'date', 'updated', 'template', etc.)
title = "Christopher Siller - Software Engineer, M.Sc." # Used by Zola for page title
description = "Christopher Siller's Curriculum Vitae - Software Engineer with experience in Big Data, Data Science, and Machine Learning." # For SEO

# Custom data for your CV, accessible in templates via `page.extra`
[extra]
name = "Christopher Siller"
cv_title = "Software Engineer, M.Sc." # Specific title for display on CV page
photo_url = "/photo.jpg" # Path to your photo in the `static` folder
pdf_file_name = "Christopher_Siller_CV.pdf" # Name for your downloadable PDF
github_pages_url = "https://ChriSil.github.io/your-cv-repo" # Your live CV URL
last_updated_display = "June 4, 2025" # Manually update or use Zola's build date in template

# Contact Facts - HTML can be rendered with `| safe` in Tera templates
[extra.facts]
Residence = "<a href='https://www.google.com/maps/place/Innsbruck/@47.2855079,11.3437708,13z/data=!3m1!4b1!4m6!3m5!1s0x479d6ecfe1f8ca73:0x9d201c7d281d9b0d!8m2!3d47.2692124!4d11.4041024!16zL20vMGZobXk'><i class='fa fa-home fact-icon'></i>Innsbruck, AT</a>"
LinkedIn = "<a href='https://www.linkedin.com/in/christophersiller/en?original_referer=https%3A%2F%2Fwww.google.com%2F'><i class='fa-brands fa-linkedin-in fact-icon'></i>Christopher Siller</a>"
GitHub = "<a href='https://github.com/ChriSil/'><i class='fa-brands fa-github fact-icon'></i>ChriSil</a>"
StackOverflow = "<a href='https://stackoverflow.com/users/7425011/chrisil'><i class='fa-brands fa-stack-overflow fact-icon'></i>ChriSil</a>"
Email = "<a href='mailto:chris.siller@alumni.fau.de'><i class='fa fa-envelope fact-icon'></i>chris.siller@alumni.fau.de</a>"
Phone = "<a href='tel:+43-670-3522557'><i class='fa fa-phone fact-icon'></i>+43 670 3522557</a>"

# Skills - structured for easy iteration and potential bar graphs
[[extra.skills]]
name = "Python"
level = 100 # Percentage for bar graph
category = "Programming & Core Tech" # Optional: for grouping in template

[[extra.skills]]
name = "Rust"
level = 30
category = "Programming & Core Tech"

[[extra.skills]]
name = "Matlab"
level = 60
category = "Data & Scientific Computing"

[[extra.skills]]
name = "Linux"
level = 80
category = "Systems & Ops"

[[extra.skills]]
name = "TensorFlow"
level = 70
category = "Machine Learning"

[[extra.skills]]
name = "Docker"
level = 70
category = "Systems & Ops"

[[extra.skills]]
name = "C++"
level = 80
category = "Programming & Core Tech"

[[extra.skills]]
name = "C#/.NET"
level = 50
category = "Programming & Core Tech"

[[extra.skills]]
name = "TypeScript"
level = 50
category = "Web & Scripting"

[[extra.skills]]
name = "Postman"
level = 40
category = "Tools"

[[extra.skills]]
name = "Jupyter"
level = 80
category = "Data & Scientific Computing"

[[extra.skills]]
name = "Kubernetes"
level = 70
category = "Systems & Ops"

# Professional Experience
[[extra.positions]]
period = "Apr 2022 - Present"
company = "Ferchau Engineering" # Using 'company' instead of 'title' for clarity
role = "Software / Data Engineer" # Using 'role' instead of 'subtitle'
location = "Innsbruck, AT"
skills_tags = ["Python", "AWS", "Docker", "Kubernetes", "Pandas", "Numpy", "Dash"] # Renamed for clarity
description = """
Part of an interdisciplinary team of Engineers, Data Scientists and Developers,
creating tools to enhance the reliability of industrial engines. The team's interest revolves around
leveraging machine learning techniques to extract new insights from the data at our disposal.
"""
key_responsibilities = [ # Renamed 'subcontents'
  "Processing and analyisis of machine and machine related data with Pandas/NumPy/SciPy.",
  "Developing Data Visualization Interfaces using Flask/Dash/Plotly.",
  "Backend Development and Data Availability with ClickHouse/Prefect/AWS/Lambda/SQL",
  "Exploring Weibull Statistics/Predictive Maintenance/RNNs/Time Series Analysis for insights."
]

[[extra.positions]]
period = "Oct 2018 – Oct 2021"
company = "Hatch Ltd."
role = "Software and Systems Engineer"
location = "Portland, OR, USA"
skills_tags = ["C++", "Python", "MatLab"]
description = """
Part of the Rail Systems Engineering group. Responsibilities revolved mainly around
development and application of TrainOps©, Hatch LTKs proprietary operations and electrical
network simulation software, as well as some related field work.
"""
key_responsibilities = [
  "TrainOps Development: feature implementation, beta testing, real world application.",
  "Postprocessing and analysis of simulation results, working on new approaches to meet high data volumes.",
  "Acquisition and preprocessing of field data to build simulation scenarios."
]

# ... (Add other positions in the same format) ...
# [[extra.positions]]
# period = "Nov 2015 – Dec 2017"
# company = "Siemens Transmission Solutions"
# ...

# [[extra.positions]]
# period = "Oct 2014 - Jul 2015"
# company = "Siemens Rail Electrification"
# ...

# [[extra.positions]]
# period = "Jun 2012 - Sep 2014"
# company = "Siemens Infrastructure and Cities"
# ...


# Education
[[extra.education_entries]] # Renamed for clarity
type = "Degree" # To distinguish from thesis section if needed
degree_info = "Master of Science, Maschinenbau"
institution = "Friedrich Alexander Universität Erlangen-Nürnberg"
period = "2015 - 2018"

[[extra.education_entries]]
type = "Degree"
degree_info = "Bachelor of Science, Maschinenbau"
institution = "Friedrich Alexander Universität Erlangen-Nürnberg"
period = "2011 - 2015"

# Theses - can be part of education or separate like your original structure
[[extra.theses]]
type = "Masters Thesis" # Was 'header'
title = "Software development to calculating flight trajectories for autonomous multicopters in intralogistics" # Was 'contents'
skills_tags = ["C++", "Python", "ROS", "Computer Vision", "Object Detection"]
description_points = [ # Was 'subcontents'
  "This project kickstarted my passion for robotics and software engineering, especially in utilizing Open Source resources. I was tasked with building the backend for an autonomous fleet or drones, and the integration of position and vision data into flight trajectory calculations.",
  "<a href='https://www.faps.fau.de/curforsch/intrafly-einsatz-autonomer-flugroboter-in-der-intralogistik/'>Intrafly Project, University of Erlangen</a>"
]

[[extra.theses]]
type = "Project Thesis"
title = "Fabrication of artficial muscles using the Aerosol-Jet-3D-Print method"
skills_tags = ["3D Print", "Aerosols", "PLC"]
description_points = [] # Empty if no subcontents

[[extra.theses]]
type = "Bachelors Thesis"
title = "Experimental and simulative analysis of thermally conductive polymers in high power LED-systems"
skills_tags = ["FEM Analysis", "Thermal Condictivity"]
description_points = []
+++

## Summary

I'm a Software Engineer with over four years of professional experience, currently working as a Software and Data Engineer in Tirol, Austria. The focus of my current project is leveraging Big Data and Data Science to enhance the performance and reliability of industrial machinery. I have a profound interest in Machine Learning, specifically Reinforcement Learning. Its potential to revolutionize various aspects of our society is both thrilling and daunting. I am intrinsically motivated to contribute meaningfully to this field.

## Additional Experience & Interests

* Some of my interests and hobbies revolve around the theory and the intricacies in machine learning. I am drawn to Reinforcement Learning projects, finding them both stimulating and rewarding. I actively engage with the AI community here in Austria to further immerse myself in the field. I am also intrigued by robotics, systems and functional programming and I enjoy customizing Linux Distributions and Kernels.
    * **Relevant Skills/Interests:** scikit-learn, PyTorch, ROS, CUDA, Rust, Arch Linux, AI Austria

* **(Currently Semi-active)** Involvement in the NNFS community. This is an effort to teach understanding of Neural Networks by building them from scratch, using Python.
    * More info: [Neural Networks from Scratch](https://nnfs.io/)
    * **Relevant Skills/Interests:** Python, NumPy, scikit-learn, PyTorch

* In 2018, I became a Registered Yoga Teacher (RYT 200) with Yoga Alliance USA. At the moment, I do not actively teach Yoga.
    * More info: [RYT @ Yoga Alliance](https://www.yogaalliance.org/Our_Standards/Elevated_RYS_200_Standards)

* I am an active member of the Academic Alpine Club Munich (AAVM) where I serve as the current President. In my free time, I like to organize climbing and mountaineering trips, and I occasionally write about them.
    * More info: [Akademischer Alpenverein München](https://www.aavm.de/index.html) (Web content update in progress.)

---