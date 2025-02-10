# 1 PRECEDENT DATA

## 1.1 Objective

Research judgments or verdicts from the Supreme Court of India for legal precedents and collect the data into a spreadsheet. You will be given a specific year and a volume from this website: https://digiscr.sci.gov.in/. Please do not work on a different year or a different volume, as other researchers would be working on those and your work if duplicate is not useful.

## 1.2 Task

Browse through each judgment/order, and identify legal precedents. Remember, we are not looking for data regarding the judgment/order, but only for the precedents in references. 

## 1.3 Deliverable

Look for the following data elements, for each precedent, and format it as the columns of a spreadsheet. Deliver the spreadsheet as an XLSX file or a CSV file.

# 2 Data Fields

## 2A (Column A) DigiSC Page URL

**Definition:**  
The official Supreme Court judgment page URL from DigiSC. Must be a full and valid URL linking directly to the judgment page.

**Examples of Allowed Entries:**
- `https://digiscr.sci.gov.in/view_judgment?id=MzEy`
- `https://digiscr.sci.gov.in/view_judgment?id=MTI3`

**Examples of Not Allowed Entries:**
- `"SC Judgment 2004 link"` (Missing URL)
- `"www.supremecourt.in/judgment"` (Incorrect format, must be from DigiSC)

---

## 2B (Column B) DigiSC PDF Link

**Definition:**  
Direct link to download the judgment PDF from DigiSC. Must be a complete and accessible URL.

**Examples of Allowed Entries:**
- `https://digiscr.sci.gov.in/admin/judgement_file/xyz.pdf`
- `https://digiscr.sci.gov.in/admin/judgement_file/abc.pdf`

**Examples of Not Allowed Entries:**
- `"Download PDF here"` (No direct URL)
- `"supremecourt.in/pdf"` (Incorrect domain, must be from DigiSC)

---

## 2C (Column C) SCR Citation

**Definition:**  
The Supreme Court Reports (SCR) citation must follow the format **[YEAR] VOLUME_NUMBER S.C.R. PAGE_NUMBER**.

**Examples of Allowed Entries:**
- `[2004] 3 S.C.R. 56`
- `[1998] 2 S.C.R. 101`

**Examples of Not Allowed Entries:**
- `"Supreme Court 2004 Ruling"` (Not in correct format)
- `"SCR Citation: Vol 3, 2004"` (Does not match required format)

---

## 2D (Column D) Neutral Citation

**Definition:**  
The neutral citation (INSC) must follow the format **[YEAR] INSC NUMBER**.

**Examples of Allowed Entries:**
- `2004 INSC 181`
- `1993 INSC 344`

**Examples of Not Allowed Entries:**
- `"2004 SC Citation"` (Incorrect format)
- `"INSC Case 344 of 1993"` (Not in the correct format)

---

## 2E (Column E) Date of Judgment

**Definition:**  
The date when the judgment was issued. It must be in **ISO 8601 format (YYYY-MM-DD)**.

**Examples of Allowed Entries:**
- `2004-03-17`
- `1993-10-27`

**Examples of Not Allowed Entries:**
- `"March 17, 2004"` (Incorrect format)
- `"17-03-2004"` (Not ISO format)

---

## 2F (Column F) Case Type

**Definition:**  
The category of the case. Use standard legal case types recognized in the Indian legal system.

**Examples of Allowed Entries:**
- `Civil Appeal`
- `Writ Petition`
- `Special Leave Petition`

**Examples of Not Allowed Entries:**
- `"Appeal"` (Too vague)
- `"Case Type: Civil"` (Incorrect format)

---

## 2G (Column G) Case Number

**Definition:**  
The unique identifier for the case. Must follow the format **X/YYYY**.

**Examples of Allowed Entries:**
- `1650/2004`
- `994/1972`

**Examples of Not Allowed Entries:**
- `"Case 1650 2004"` (Incorrect format)
- `"1650-2004"` (Wrong separator)

---

## 2H (Column H) Disposal Nature

**Definition:**  
The final outcome of the case, indicating whether the appeal was allowed, dismissed, or otherwise disposed of.

**Examples of Allowed Entries:**
- `Appeals Allowed`
- `Appeals Dismissed`

**Examples of Not Allowed Entries:**
- `"Judgment Issued"` (Not specific enough)
- `"Case Completed"` (Not a legal term)

---

## 2I (Column I) Order/Judgment

**Definition:**  
Specifies whether the document is an "Order" or a "Judgment."

**Examples of Allowed Entries:**
- `Judgment`
- `Order`

**Examples of Not Allowed Entries:**
- `"Verdict"` (Not a standard legal term)

---

## 2V (Column V) Legal Principle

**Definition:**  
A brief summary of the main legal principle derived from the case.

**Examples of Allowed Entries:**
- `"Fraudulent misrepresentation voids contracts."`
- `"A contract obtained through coercion is void."`

**Examples of Not Allowed Entries:**
- `"The case was about fraud."` (Too vague)
- `"General legal discussion."` (Not specific)

---

## 2W (Column W) Q1 (Most Important Legal Question)

**Definition:**  
The most important legal question the judgment answers. It should be phrased in a way that someone might search for it online.

**Examples of Allowed Entries:**
- `"What are the consequences of suppressing material facts in court?"`
- `"Can a fraudulent misrepresentation void a contract?"`

**Examples of Not Allowed Entries:**
- `"Did Mr. X suppress evidence?"` (Should not include names)
- `"Was fraud committed?"` (Too vague)

---

## 2X (Column X) Q1 Location

**Definition:**  
The page and paragraph number where Q1 is discussed in the judgment.

**Examples of Allowed Entries:**
- `Page 672, Paragraph 16`
- `Page 108, Paragraph 4`

**Examples of Not Allowed Entries:**
- `"In the middle of the document"` (Not specific enough)

---

## 2AC (Column AC) Primary Legal Question

**Definition:**  
The most significant legal issue addressed in the judgment. It should be framed as a legal principle.

**Examples of Allowed Entries:**
- `"What are the consequences of suppressing material facts?"`
- `"What is the effect of fraud on court proceedings?"`

**Examples of Not Allowed Entries:**
- `"Is the plaintiff guilty?"` (Should be legal, not factual)

---

## 2AE (Column AE) Tertiary Legal Question

**Definition:**  
The third key legal issue addressed by the case.

**Examples of Allowed Entries:**
- `"Is a judgment obtained by fraud considered a nullity?"`
- `"Can trustees delegate their duties and powers?"`

**Examples of Not Allowed Entries:**
- `"Did the judge favor the respondent?"` (Not a legal issue)






## 2x (Column X) DigiSCR Page URL

The URL of the webpage. You may not be able to directly get this URL. You will have to click through a judgment that cites this precedent. Usually precedents are listed in a section called **Case Law Cited** For example, look below:





## 2x (Column X) Indian Laws Referenced

List laws/sections that the precedent references. Use format: The, law name, year.

If the precedent references more than one law, list *all* the laws in this column, separated by *semicolons*.

Examples:
- *The Code of Civil Procedure, 1908*
- *The Indian Trusts Act, 1882*
- *The Constitution of India, 1950*

## 2x (Column X) Critical Question

B. What is the most critical question that this judgment answers? It should be stated generically, as a general question someone might search for online. Avoid using names; instead, refer to individuals as "litigants."

C. What is the second most important question that this judgment answers? It should be stated generically, as a general question someone might search for online. Avoid using names; instead, refer to individuals as "litigants."

D. What is the third most crucial question that this judgment answers? It should be stated generically, as a general question someone might search for online. Avoid using names; instead, refer to individuals as "litigants."

E. What classification does the First Party have? Determine if the first party is an appellant, petitioner, plaintiff, respondent, defendant, or another type of "litigant."

F. What is the full name of the First Party: first name, middle name, and last name? If only initials are present, do not include periods between the letters. If there is any language like "& ors," substitute with "and others."

G. What classification does the Second Party have? Determine if the first party is an appellant, petitioner, plaintiff, respondent, defendant, or another type of "litigant."

H. What is the full name of the Second Party: first name, middle name, and last name? If only initials are present, do not include periods between the letters. If there is any language like "& ors," substitute with "and others."

I. Just put the value "Supreme Court of India."

J. What Type of Case Is It? – For example, Special Leave Petition, Civil Appeal, Criminal Appeal, Writ Petition, Criminal Miscellaneous Petition, Criminal Case, etc. Please use a standardized data format commonly utilized in the Indian legal system, and try to avoid abbreviations or shortening phrases.

K. What is the case number? Format must be X/YYYY. Do not indicate the type of case (abbreviations or shortened phrases or alphabets) in this field.

L. What is the date of the judgment or verdict? Use ISO 8601 standard for formatting the date as YYYY-MM-DD, plus capital letter T. So a date would look like 2024-01-02T.

M. Who are the judge(s) involved in the Bench who gave the judgment, listed and separated by semicolons? First name, middle name, and last name? If only initials are present, do not include periods between the letters.

N. Who is the author of the judgment? The name(s) of the judge(s). first name, middle name, and last name? If only initials are present, do not include periods between the letters.

O. Who was the judgment in favor of? The appellant, petitioner, plaintiff, respondent, defendant, or "other party"?

P. Link to Judgment on digital supreme court report. To get the link, click on the case name, then click on the FULL TEXT button on the right-handside of the screen. Once the PDF loads, just get the URL in the browser address bar. The URL will appear in this format https://digiscr.sci.gov.in/admin/judgement_file/judgement_pdf/2004/volume%203/Part%20I/2004_3_56-67%20%20%20_1703307014.pdf

Q. Link to Judgment on IndianKanoon.org (Provide the full URL starting with "https://," no hyperlink text.)

R. The citation number from the Supreme Court Cases (SCC) should be standardized as follows: (YEAR) VOLUME_NUMBER SCC PAGE_NUMBER. It is essential to adhere strictly to this format; no other formats may be used. You may need to conduct thorough research online to obtain this information.

S. The Supreme Court Reports (S.C.R.) citation number's format should be: [YEAR] VOLUME_NUMBER S.C.R. PAGE_NUMBER. It is essential to adhere strictly to this format; no other formats may be used. You may need to conduct thorough research online to obtain this information.

T. The citation number from the INSC should be standardized as follows: [YEAR] INSC NUMBER. It is essential to adhere strictly to this format; no other formats may be used. You may need to conduct thorough research online to obtain this information.

U. The All India Reporter (AIR) citation number is standardized: AIR YEAR SC PAGE_NUMBER. It is essential to adhere strictly to this format; no other formats may be used. You may need to conduct thorough research online to obtain this information.

V. The citation number from the Judgment Today standardized as follows: JT VOLUME_NUMBER SC PAGE_NUMBER or JT(Suppl) VOLUME_NUMBER SC PAGE_NUMBER. It is essential to adhere strictly to this format; no other formats may be used. You may need to conduct thorough research online to obtain this information.

W. The citation number from the SCALE standardized as follows: YEAR VOLUME_NUMBER SCALE PAGE_NUMBER. It is essential to adhere strictly to this format; no other formats may be used. You may need to conduct thorough research online to obtain this information.

X. The citation must be in this column if it is not from SCC, S.C.R., INSC, AIR, JT, or SCALE.

Y. The legal principle of the case

Z. A quote from the case that establishes the legal principle. All quotes must be verbatim, word for word.

AA: The location of the quote in the judgment. For example, in the PDF file of the page 234, paragraph 2

AB. A second quote from the case that establishes the legal principle. All quotes must be verbatim, word for word.

AC: The location of the second quote in the judgment. For example, in the PDF file of the page 234, paragraph 2

AD. A third quote from the case that establishes the legal principle. All quotes must be verbatim, word for word.

AE: The location of the third quote in the judgment. For example, in the PDF file of the page 234, paragraph 2

Please ensure that if you are not entirely confident about the information in fields E to X, you should suffix the data with an asterisk. If any information is unavailable, leave that field blank. If you are only partially specific about the data, you can also provide that information, marked with an asterisk.

The results should be in a table format consisting of two rows and twenty-three columns in an EXCEL file. The first row must include columns labeled A through AE. The second row onwards should contain the data obtained from your research.

Accuracy: The data you collect must be 97% accurate. If you deliver a row of 31 columns, only two columns can be inaccurate. More than this, the row will be rejected.

You must check the data manually. Please note that you can use AI tools to collect data, but most of them also deliver false data. So, be sure to double-check the data that AI tools give you. Using AI tools will not be an excuse for providing inaccurate data.

Completeness: Your data must be at least 85% complete. If you deliver a row of 31 columns, you must have at least 26 correct values. If there are less than 26 values, the row will be rejected. 

Please download the data sample for examples of how to collect data. But please remember that data samples might have errors. That does not mean that your delivery can have errors. 
