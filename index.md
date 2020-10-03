---
layout: default
---

<div id="mobile-menu-open" class="shadow-large">
    <i class="fa fa-bars" aria-hidden="true"></i>
</div>
<!-- End #mobile-menu-toggle -->
<header>
    <div id="mobile-menu-close">
        <span>Close</span> <i class="fa fa-times" aria-hidden="true"></i>
    </div>
    <ul id="menu" class="shadow">
        <li>
            <a href="#about">About</a>
        </li>
        <li>
            <a href="#experience">Experience</a>
        </li>
        <li>
            <a href="#education">Education</a>
        </li>
        <li>
            <a href="#projects">Projects</a>
        </li>
        <li>
            <a href="#skills">Skills</a>
        </li>
        <li>
            <a href="#contact">Contact</a>
        </li>
    </ul>
</header>
<!-- End header -->

<div id="lead">
    <div id="lead-content">
        <h1>Sidharth Mehta</h1>
        <h2>Computer Engineer</h2>
        <a href="./documents/Sidharth Mehta.pdf" class="btn-rounded-white">View Resume</a>
    </div>
    <!-- End #lead-content -->

    <div id="lead-overlay"></div>

    <div id="lead-down">
        <span>
            <i class="fa fa-chevron-down" aria-hidden="true"></i>
        </span>
    </div>
    <!-- End #lead-down -->
</div>
<!-- End #lead -->

<div id="about">
    <div class="container">
        <div class="row">
            <div class="col-md-4">
                <h2 class="heading">About Me</h2>
            </div>
<div class="col-md-8" markdown="1">
I am Graduate Computer Engineering student at North Carolina State University looking for positions in domain of Embedded Systems and Software development.

As part of my master's degree I have worked on the following:
1. Preemptive scheduling using RTOS and Non preemptive scheduling by breaking tasks into Finite State Machines.
1. Optimizing code on embedded systems for speed, responsiveness, memory and power.
1. C++ based simulators for components of processor like cache, branch predictors and out of order processor pipeline.
1. Best practices for design of ASICs with help of Verilog.
1. Understanding how compilers perform optimization and enabling compiler to produce efficient object code.
1. Optimization of code on Linux based embedded systems with help of SIMD instructions.
1. Implementing serial communication protocols such as I2C, SPI, USB and UART.
1. Basic concepts and mechanisms related to the design of modern operating systems (process creation, threads, scheduling, synchronization).
1. Techniques to decompose and divide a program for parallel execution using OpenMP.
</div>
        </div>
    </div>
</div>
<!-- End #about -->

<div id="experience" class="background-alt">
    <h2 class="heading">Experience</h2>
    <div id="experience-timeline">
        <div data-date="June 2017 – November 2017">
<div markdown="1">
### EMTECH Foundation
#### Embedded systems Intern
EMTECH Foundation is an embedded systems training and consultancy company. As part of my internship I undertook the following responsibilities:
* Schematic and PCB design for various projects using Altium designer.
* Writing firmware for projects based on PIC and STM32 microcontroller.
* Proof-reading and quality maintenance of technical documents.
* Assisting students undergoing embedded systems training at EMTECH Foundation.
</div>
        </div>
    </div>
</div>
<!-- End #experience -->

<div id="education">
    <h2 class="heading">Education</h2>
    <div class="education-block">
        <h3>North Carolina State University</h3>
        <span class="education-date">August 2019 - May 2020</span>
        <h4>Masters of Science in Computer Engineering</h4>
        <p>
            <b>Coursework: </b>
            Architecture of Parallel computers, Object Oriented Design and Development, Operating systems, Real Time Embedded System, Embedded System Optimization, Embedded Linux, Compilers, Microprocessor Architecture, ASIC and FPGA design with Verilog
        </p>
    </div>
    <!-- End .education-block -->

    <div class="education-block">
        <h3>YMCA University of Science and Technology</h3>
        <span class="education-date">August 2014 - June 2018</span>
        <h4>Bachelor of Technology in Electronics and Communication Engineering</h4>
    </div>
    <!-- End .education-block -->
</div>
<!-- End #education -->

<div id="projects" class="background-alt">
    <h2 class="heading">Projects</h2>
    <div class="container">
        <div class="row">
            {% for project in site.data.content.projects %}

            <div class="project shadow-large">
                <div class="project-image">
                    <img src="{{ project.image }}" />
                </div>
                <!-- End .project-image -->
                <div class="project-info">
                    <h3>{{ project.name }}</h3>
                    <p>{{ project.info }}</p>
                    {% if project.url and project.url != '' %}
                    <a href="{{ project.url }}">View Project</a>
                    {% endif %}
                </div>
                <!-- End .project-info -->
            </div>
            <!-- End .project -->
            {% endfor %}
        </div>
    </div>
</div>
<!-- End #projects -->

<div id="skills">
    <h2 class="heading">Skills</h2>
    {% for skill in site.data.content.skills %}
        <h3>{{ skill.name }}</h3>
        <ul>
        {% for item in skill.keywords %}
            <li>{{ item }}</li>
        {% endfor %}
        </ul>
    {% endfor %}
</div>
<!-- End #skills -->

<div id="contact">
    <h2>Get in Touch</h2>
    <div id="contact-form">
        <form method="POST" action="https://formspree.io/sidharthmehta@outlook.com">
            <input type="hidden" name="_subject" value="Contact request from personal website" />
            <input type="email" name="_replyto" placeholder="Your email" required>
            <textarea name="message" placeholder="Your message" required></textarea>
            <button type="submit">Send</button>
        </form>
    </div>
    <!-- End #contact-form -->
</div>
<!-- End #contact -->

<footer>
    <div class="container">
        <div class="row">
            <div class="col-sm-5 copyright">
                <p>
                    2020 Sidharth Mehta
                </p>
            </div>
            <div class="col-sm-2 top">
                <span id="to-top">
                    <i class="fa fa-chevron-up" aria-hidden="true"></i>
                </span>
            </div>
            <div class="col-sm-5 social">
                <ul>
                    <li>
                        <a href="https://github.com/SidharthMehta" target="_blank"><i class="fa fa-github"
                                aria-hidden="true"></i></a>
                    </li>
                    <li>
                        <a href="https://www.linkedin.com/in/sidharthmehta1996/" target="_blank"><i class="fa fa-linkedin"
                                aria-hidden="true"></i></a>
                    </li>
                    <li>
                        <a href="mailto:sidharthmehta@outlook.com" target="_blank"> <i class="fa fa-envelope" aria-hidden="true"></i> </a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</footer>
<!-- End footer -->

<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
<script src="js/scripts.min.js"></script>
