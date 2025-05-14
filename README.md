### A reminder

The start of each message ID was changed to ```SkyMansion-```. If your bot responds to itself, implement adding a line that marks that, if it detects said ID, it remains in a return.

```Javascript

/* 
Regularly used method 
*/
let m.isBot = m.id.startsWith('BAE5') && m.id.length === 16 || m.id.startsWith('3EB0') && m.id.length === 12 || m.id.startsWith('3EB0') && (m.id.length === 20 || m.id.length === 22) || m.id.startsWith('B24E') && m.id.length === 20;



/* 
Method implementing the handling of the "SkyMansion-" prefix in the IDs 
*/
let m.isBot = m.id.startsWith('SkyMansion-') || m.id.startsWith('BAE5') && m.id.length === 16 || m.id.startsWith('3EB0') && m.id.length === 12 || m.id.startsWith('3EB0') && (m.id.length === 20 || m.id.length === 22) || m.id.startsWith('B24E') && m.id.length === 20;

if (m.isBot) return;

```
#### Credit - Baileys by ds6 (https://github.com/ds6/bails)
