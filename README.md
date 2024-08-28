**Description:**


CSV Injection on the api /product/{id}/edit or /product/add with param "name" of Defectdojo version 2.37.3 ([https://github.com/DefectDojo/django-DefectDojo](https://github.com/DefectDojo/django-DefectDojo)) allow remote attackers to insert malicious code. When user execute export product with type csv. When executed open file immediately malicious code is executed.

**Proof of Concept:**
1. Add new or edit product with param name injected with malicious code
2. Export product with type csv
3. Open the csv file that was just downloaded. The malicious code is immediately executed.




![image](https://github.com/user-attachments/assets/f420021e-5b83-49e1-9ed9-0103fbdc85d1)
![image](https://github.com/user-attachments/assets/5560af45-c8d7-44c0-8d4f-78be0ade6274)
![image](https://github.com/user-attachments/assets/e24c5775-2244-40a4-883b-1237e55c556f)
![image](https://github.com/user-attachments/assets/d7c95263-b97c-4d82-9ebb-fdc025480b03)
![image](https://github.com/user-attachments/assets/3baa0cb8-889d-4363-8e05-dd7e55dbecb1)
![image](https://github.com/user-attachments/assets/69464e6f-cec5-41a7-897b-9b1cc87142b6)


**Impact:**


Execution of Malicious Code
