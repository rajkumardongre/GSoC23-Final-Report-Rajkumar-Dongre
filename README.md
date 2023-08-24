<p align="center">
    <img src="https://upload.wikimedia.org/wikipedia/commons/a/a7/GSoC-logo-horizontal.svg" width="600px" />
</p>
<p align="center"  style="font-size:2.5rem">
    <img src="https://upload.wikimedia.org/wikipedia/commons/b/b8/Fortran_logo.svg" style="width:100px;padding-right:0.5rem;"/>
</p>

<div style="text-align: center;margin:0px;padding:0px;width:100%">
    <h1 >GSoC 2023 : Final Report</h1> 
</div>

## Project Details

- **Organization:** Fortran-Lang
- **Project:** [High-level HTTP client library](https://github.com/fortran-lang/http-client)
- **Mentors:** Milan Curcic, Arteev Raina, Philipp Engel
- **Contributor:** Rajkumar Dongre

This report summarizes the work done as part of my `GSoC 2023` project titled `High-level HTTP client library` at [**`fortran-lang/http-client`**](https://github.com/fortran-lang/http-client).

## Abstract:
The primary focus of this project was to connect the world of Fortran programming with the realm of HTTP communication. Through the creation of a high-level HTTP request library, the project aimed to equip Fortran programmers with a user-friendly toolkit for seamlessly executing standard HTTP requests. This encompassed an array of request methods, notably including popular choices such as `GET`, `HEAD`, `POST`, `PUT`, `PATCH`, and `DELETE`. The project's intent was to facilitate smooth integration of HTTP interactions into Fortran applications, simplifying the traditionally complex process and promoting enhanced connectivity between Fortran and web services.

## Project Overview

The project's primary objective was to create a high-level library for HTTP requests that caters specifically to the Fortran programming language. To achieve this, the project utilized the existing [fortran-curl](https://github.com/interkosmos/fortran-curl) library, which provides Fortran bindings to the powerful [libcurl](https://curl.se/) library—a widely adopted tool for handling HTTP requests.

The overarching goals of the project included:

1. **HTTP Request Abstraction:** Develop a user-friendly interface that abstracts the complexities of forming HTTP requests. This abstraction aimed to shield Fortran developers from the intricacies of crafting HTTP headers, managing timeouts, and dealing with various HTTP response codes.

2. **Support for Common HTTP Methods:** Implement functions within the library that correspond to standard HTTP methods. Each function was designed to accept relevant parameters and payload data where applicable, providing a cohesive way to initiate various types of requests.

3. **Response Handling and Parsing:** Create mechanisms to retrieve and parse data from the response body and headers. This functionality would enable Fortran programmers to efficiently extract and process valuable information from HTTP responses.

4. **Integration with "fortran-curl":** Leverage the existing "fortran-curl" library to establish the underlying connection and communication with web services. This integration was pivotal in harnessing the power of the battle-tested "libcurl" library and extending its capabilities to the Fortran domain.

5. **Ease of Use:** Prioritize user experience by designing the library with simplicity and usability in mind. The aim was to lower the barrier of entry for Fortran developers who may have limited prior experience with web interactions.

6. **Test Cases and Quality Assurance:** Implement a comprehensive suite of test cases to ensure the robustness and reliability of the library's functionalities. Test cases were crafted to cover a range of scenarios, including different HTTP methods, response codes, payload types, and edge cases. The integration of automated testing aimed to identify and rectify potential issues early in the development process.

7. **Documentation and Examples:** Create comprehensive documentation and examples that guide developers through the process of incorporating the library into their Fortran projects. This facet aimed to empower developers to quickly grasp the library's functionality and integrate it effectively.

## Progress and Accomplishments

Throughout the Google Summer of Code 2023 program, significant strides were made in achieving the core goals of the project. The following sections highlight the major accomplishments, technical advancements, and features that were successfully implemented.

**Features of the Library:**

The developed high-level HTTP library for Fortran boasts a range of features designed to empower developers in making seamless HTTP requests and interacting with web services. These features include:

1. **Sending HTTP Requests:**
   - **GET:** Retrieve data from the server.
   - **POST:** Submit data to be processed by the server.
   - **PUT:** Replace or create resources on the server.
   - **DELETE:** Remove resources from the server.
   - **PATCH:** Perform partial updates to resources.
   - **HEAD:** Retrieve response headers without the response content.

2. **Data Support:**
   - The library accommodates the sending of various data types with requests, supporting file uploads and form data.

3. **Response Handling:**
   - Developers can retrieve response content effortlessly.
   - The HTTP status code returned by the server can be obtained for proper status handling.
   - The length of the response content can be fetched to manage data streams effectively.
   - Access to response headers facilitates the extraction of crucial information.

4. **Custom Headers:**
   - Developers can include custom headers in requests to the server, enhancing flexibility in interactions.

5. **Error Handling:**
   - Unsuccessful requests are detected and handled gracefully, accompanied by informative error messages that aid in debugging.

6. **Request Timeout:**
   - A crucial enhancement for responsiveness, the ability to set a maximum time allowed for request completion was implemented.

7. **Authentication:**
   - Standard authentication methods are supported, allowing requests to protected resources with appropriate authentication credentials.

**Accomplishments:**

- **HTTP Methods Implementation:** All standard HTTP request methods were successfully implemented within the library, enabling developers to seamlessly interact with web services using a familiar syntax.

- **Response Parsing:** Mechanisms for parsing data from both response bodies and headers were developed, providing developers with the ability to extract and process essential information from server responses.

- **Automated Testing:** A comprehensive suite of automated tests was established to ensure the library's functionalities were robust and reliable. These tests covered diverse scenarios, including various HTTP methods, response codes, payload types, and edge cases.

- **Documentation:** Comprehensive documentation was created, including usage guides, examples, and API references. This documentation empowers developers to quickly grasp and integrate the library into their projects.

- **Integration with "fortran-curl":** The seamless integration of the library with the "fortran-curl" bindings to "libcurl" ensured efficient underlying communication with web services.

- **Usability Enhancement:** By abstracting the complexities of low-level HTTP interactions, the library significantly improved the accessibility of web services for Fortran programmers, simplifying their development process.

## Learning and Skill Development

Participation in the Google Summer of Code 2023 provided a rich and immersive learning experience, fostering the acquisition of valuable skills and knowledge in various domains. The journey encompassed not only the project's technical aspects but also the broader ecosystem of software development and collaboration. The following areas outline the key learning points during the program:

- **Version Control with Git and GitHub:**
  Through continuous collaboration and version tracking using Git and GitHub, I honed my proficiency in maintaining codebase history, handling merge conflicts, and efficiently collaborating with other contributors.

- **Continuous Integration and Continuous Deployment (CI/CD):**
  The integration of CI/CD pipelines into the development workflow familiarized me with the importance of automated testing, code quality checks, and the seamless deployment of code changes. This knowledge contributes to producing robust and reliable software.

- **Fortran Language Fundamentals and Best Practices:**
  Working extensively with Fortran provided an opportunity to deepen my understanding of the language's syntax, idioms, and best practices. I gained insights into writing clean, efficient, and maintainable Fortran code.

- **Fortran Package Management:**
  Exploring Fortran package management systems equipped me with the skills to efficiently manage dependencies, incorporate external libraries, and ensure smooth collaboration in the Fortran ecosystem.

- **Network Programming and HTTP:**
  Delving into network programming concepts and the intricacies of the HTTP protocol allowed me to grasp the underlying mechanisms of web interactions. This understanding was essential for building a robust and effective HTTP library.

- **Integration of libcurl and Curl:**
  Integrating "libcurl" and "curl" libraries into the Fortran environment exposed me to the intricacies of low-level network communication, further enhancing my programming prowess.

The learning process extended beyond technical skills and encompassed essential soft skills as well. Communication, time management, adaptability, and problem-solving were consistently refined through interactions with mentors, engaging in discussions with the open-source community, and navigating project complexities.

Engaging with the Fortran community and contributing to open-source projects deepened my appreciation for collaborative development, the value of code reviews, and the importance of maintaining an open and inclusive environment for contributors of varying skill levels.

As the Google Summer of Code 2023 program concludes, the knowledge gained and experiences amassed will undoubtedly prove instrumental in my continued journey as a software developer. The skills and insights acquired not only enhance my technical repertoire but also shape my approach to tackling future challenges in the ever-evolving landscape of software engineering.

**Future Work**

The completion of the Google Summer of Code 2023 project marks a significant milestone in the development of the high-level HTTP library for Fortran. However, there are several avenues for further enhancement and expansion that could be explored in the future. The following areas represent potential directions for future work:

1. **Extended HTTP Features:**
   While the current library provides support for the most common HTTP methods, there is room for expansion to accommodate more specialized methods and features, such as handling redirects, managing cookies, and implementing more advanced authentication mechanisms.

2. **User Authentication Flow Simplification:**
   Simplifying the process of integrating authentication tokens, such as OAuth tokens, could make authentication with protected resources even more straightforward for developers.

3. **Integration with More Libraries:**
   While the project currently relies on "fortran-curl" for handling HTTP interactions, exploring integrations with other Fortran libraries or tools might offer alternative approaches to achieving similar goals.

4. **Wider Platform Compatibility:**
   Extending the library's compatibility to a broader range of platforms and compilers could ensure that a wider audience can leverage its capabilities without constraints.

5. **Community Engagement and Documentation Expansion:**
   Encouraging community contributions, expanding documentation with additional examples and use cases, and fostering discussions could lead to a more vibrant ecosystem around the library.

These potential avenues for future work illustrate the project's potential for growth and further impact. As the project continues to evolve, it has the opportunity to address more complex use cases, cater to diverse developer needs, and contribute to the Fortran community's ongoing progress in web interactions.

**Acknowledgments**

The successful culmination of this Google Summer of Code 2023 project was made possible through the guidance, support, and contributions of numerous individuals and the collective efforts of the open-source community. I extend my heartfelt gratitude to Milan Curcic, Arteev Raina, Philipp Engel, Jeremie Vandenplas and Ubaid Shaikh whose guidance and mentorship were invaluable throughout this journey. I am also grateful to my peer Saurabh Suresh Powar.

I would also like to express my gratitude to the broader open-source community, whose resources, discussions, and collective knowledge have been an invaluable source of inspiration and assistance.

Additionally, I am thankful to Google for organizing the Google Summer of Code program, providing a platform that fosters learning, collaboration, and the opportunity to contribute meaningfully to open-source projects.

Finally, to my fellow contributors, testers, and anyone who offered support, encouragement, or insights, I extend my heartfelt appreciation. This project truly stands as a testament to the power of collaboration and shared dedication.

Thank you all for your contributions, mentorship, and support in making this project a reality. Your guidance has not only enriched my technical skills but has also been pivotal in shaping my growth as a software developer.

