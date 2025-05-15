# SOFTWARE REQUIREMENTS SPECIFICATION(SRS) DOCUMENT

## Parts of a SRS document

The important parts of SRS document are: 

### Functional requirements of the system

The functional requirements section of the SRS breaks down the functionalities required from the system. 

Functional requirements describe a set of high-level requirements, where each high-level requirement takes some data from the user and provides some data to the user as an output. Also each high-level requirement might consist of several other functions. 

The system is considered to perform a set of high-level functions where each function of that system can be considered as a transformation of a set of input data to the corresponding set of output data. The deliverable being, a user interacting with this system being able to get some meaningful piece of work done using this system's high-level functions. 

The high-level functional requirements often need to be identified either from an informal problem description document or from a conceptual understanding of the problem. Each high- level requirement characterizes a way of system usage by some user to perform some meaningful piece of work. 

**Example: -** Consider the case of a human resource Information system, where –**F1:** Search Employee functionInput: an Employee’s nameOutput: the employee profile, position, designation and other related employee information within the HRIS.

So the function Search Employee (F1) takes the Employee's name and transforms it into Employee details. 

There can be many types of users of a system and their requirements from the system may be very different. So, it is often useful to identify the different types of users who might use the system and then try to identify the requirements from each user’s perspective. 

When documenting the functional requirements, we need to specify the set of functionalities supported by the system. A function can be specified by identifying the state at which the data is to be input to the system, its input data domain, the output data domain, and the type of processing to be carried on the input data to obtain the output data. 

 Consider documenting the withdraw-cash function of an ATM (Automated Teller Machine) system. 

The withdraw-cash is a high-level requirement. It has several sub-requirements corresponding to the different user interactions. These different interaction sequences capture the different scenarios. 

Example: - Withdraw Cash from ATM 
R1: withdraw cash 
Description: The withdraw cash function first determines the type of account that the user has and the account number from which the user wishes to withdraw cash. It checks the balance to determine whether the requested amount is available in the account. If enough balance is available, it outputs the required cash; otherwise it generates an error message. 

R1.1 select withdraw amount optionInput: “withdraw amount” optionOutput: user prompted to enter the account type 

R1.2:  select account type 
Input: user option Output: prompt to enter amount 
R1.3:  get required amount Input: amount to be withdrawn in integer values greater than 100 and less than 10,000 in multiples of 100. Output: The requested cash and printed transaction statement. Processing: the amount is debited from the user’s account if sufficient balance is available, otherwise an error message displayed. 




### Non-functional requirements of the system

Nonfunctional requirements deal with the characteristics of the system which cannot be expressed as functions - such as the maintainability of the system, portability of the system, usability of the system, etc. 


### Goals of implementation 

The goals of implementation section documents some general suggestions regarding development. These suggestions guide trade-off among design goals. The goals of implementation section might document issues such as revisions to the system functionalities that may be required in the future, new devices to be supported in the future, reusability issues, etc. These are the items which the developers might keep in their mind during development so that the developed system may meet some aspects that are not required immediately. 


## Properties of a good SRS document 

The important properties of a good SRS document are the following: 

* **Concise**. The SRS document should be concise and at the same time unambiguous, consistent, and complete. Verbose and irrelevant descriptions reduce readability and also increase error possibilities. 

* **Structured**. It should be well-structured. A well-structured document is easy to understand and modify. In practice, the SRS document undergoes several revisions to cope up with the customer requirements. Often, the customer requirements evolve over a period of time. Therefore, in order to make the modifications to the SRS document easy, it is important to make the document well-structured. 

* **Black-box view**. It should only specify what the system should do and refrain from stating how to do these. This means that the SRS document should specify the external behavior of the system and not discuss the implementation issues. The SRS document should view the system to be developed as black box, and should specify the externally visible behavior of the system. For this reason, the SRS document is also called the black-box specification of a system. 

* **Conceptual integrity**. It should show conceptual integrity so that the reader can easily understand it. 
* **Response to undesired events**. It should characterize acceptable responses to undesired events. These are called system response to exceptional conditions. 
* **Verifiable**. All requirements of the system as documented in the SRS document should be verifiable. This means that it should be possible to determine whether or not requirements have been met in an implementation. 
## 	Problems without a SRS document 
The important problems that an organization would face if it does not develop a SRS document are as follows: 
* Without developing the SRS document, the system would not be implemented according to customer needs. 
* Software developers would not know whether what they are developing is what exactly required by the customer. 
* Without SRS document, it will be very much difficult for the maintenance engineers to understand the functionality of the system. 
* It will be very much difficult for user document writers to write the users’ manuals properly without understanding the SRS document. 
 
## Problems with an unstructured specification 

* It would be very much difficult to understand that document.
* It would be very much difficult to modify that document.
* Conceptual integrity in that document would not be shown.
* The SRS document might be unambiguous and inconsistent. 


## Freely available SRS examples (including some for open source software): 

• SRS for apps and a data repository for distributing manu- facturing data: Thomas Hedberg Jr., Moneer Helu, and Mar- cus Newrock (Dec. 2017). Software Requirements Specifica- tion to Distribute Manufacturing Data. https://web.archive. org / web / 20201208070659 / https : / / nvlpubs . nist . gov/nistpubs/ams/NIST.AMS.300-2.pdf 
• SRS for data system that assesses conservation practices:Data System Team (n.d.). System Requirements Specificationfor STEWARDS. https://web.archive.org/web/20200923200038/ https://www.nrcs.usda.gov/Internet/FSE_DOCUMENTS/ nrcs143_013173.pdf 
• SRS for an app that splits and merges PDFs: Ploutarchos Spyridonos (Feb. 2010). Software Requirements Specification for PDF Split and Merge, Version 2.1.0. https : / / web . archive . org / web / 20170225043950 / http : / / selab . netlab.uky.edu/%7Eashlee/cs617/project2/PDFSam. pdf 
• SRS for software that processes EEG data: Inria InnovationLab (n.d.). Software Requirement Specification for CertiViBE,v1.0. https://web.archive.org/web/20190710221933/ http://openvibe.inria.fr/openvibe/wp-content/ uploads/2018/04/CERT-Software-Requirement-Specification. pdf 
• SRS for library software: Fred Eaker (Nov. 2006). Soft-ware Requirements Specification for Vyasa. https://web.archive . org / web / 20161127184329 / http : / / vyasa . sourceforge.net/vyasa_software_requirements_specification. pdf 





