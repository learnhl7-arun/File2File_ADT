# File2File_ADT
Sample Mirth Connect Project – HL7 2.x Transformation (2.3 to 2.4)

Input Channel is a File Reader. 
Output Channel is File Writer. 

The input is a 2.3 message and is transformed into a 2.4 message. 

This channel does the following
- Set the HL7 version to 2.4
- Reassign the Sender ID to Mirth
- Update the Date and Time to current in the MSH segment
- Pad the Date and Time with 00’s for seconds in the EVN segment
- Force the Admit Reason to be uppercase
- Enforce a list of Genders for the destination.  If we hit an unexpected gender, we’ll assign it as “O” for other.  



