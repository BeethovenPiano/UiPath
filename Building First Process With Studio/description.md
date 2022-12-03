Building First Process With Studio

-> This workflow retrieves all unread emails,from the Outlook account in use that have 'Course Invoices' in the subject line.
-> Emails retrieved are saved under the 'CourseEmails' list MailMessage type of variable.
-> Afterwards, attachements for each mail message retrieved are saved in a new project folder titled "Invoices".
-> It then identifies and copies the client code from each attachment and stores it under the 'ClientCode' variable.
-> Next, using the Edge browser , it access the "https://acme-test.uipath.com/first-automation" webpage, click 'Part2'
   and types in the client code to   get the discount value.
-> The disount value is stored under the 'DiscountValue' variable (this operation is repeated for all stored client codes).
-> If the discount value contains the "$" character the value will be typed in the "Invoice" sheet, in the "E18" cell. Otherwise, the value "$0" will be added.
-> Next, the "RPA Dev, RPADeveloper@uipath.com" signature is added in each of the invoice sheets.
-> Finally, write the text to be used to prepare an Outlook draft email containing the uploaded invoices (the draft email can be found inside the 
  "Drafts" folder of the Outlook account in use).
-> Published the process to the Orchestrator 
-> Runed the published process through the UiPath assistance.
