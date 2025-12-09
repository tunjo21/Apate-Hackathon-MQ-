# Apate-Hackathon-MQ-
UI/UX Principles for APATE Investigation Scam Leads Portal

Summary: 
This prototype is a lightweight web-based portal designed to help fraud analysts review captured scam leads, understand and display asssociated metadata
and allow them to take appropriate investigative actions. The prototype delivers a clean UI driven by real analyst workflows, mock data for simulating real leads
and action buttons for quick remediation and triage. These actions include Escalate, Ignore and Investigate. Overall, the main focus of this prototype is to deliver an interface that is 
efficient, safe, intuitive and purpose-built for investigating scam leads.

Applied UI/UX Principles
1. Clarity and Hierarchy:
   Our design aims keep the prototype clean and simple, intentionally avoiding clutter for easy display and navigation. Its minimalistic design ensures
   only essential data is displayed as required, including risk ID, scam type, the location in which it occurred and its action status. Color coding is also used
   consistently, since each risk level is highlighted with a different color. Status icons have other distinct colors(open - blue, ignored - grey and investigating - purple) to
   further distinguish them. Table headers are also displayed to be more larger, while rows are separated with spacing. Action buttons are grouped for quick scanning. 

2. Consistency:
   The interface uses one font(Montserrat) for readability and professionalism across all components. Buttons share a consistent shape
   (rounded, pill shaped for actions and rectangular for modals). Modal windows themselves follow the same layout throughout the interface: title, content
   and actions.

3. Status Feedback:
   The table rows and action buttons use a hover state(are raised slightly) to provide a quick and interactive response to the
   user. The modals open and close clearly with smooth transitions, while the empty state prevents any confusion when there is no
   data available.

4. Responsiveness:
   Every icon/button has an appropriate response(light/dark switches to the mode in alternate clicks, add button adds more scam lead entries).
   The search bar near the top also allows for quick response and displays the entry in seconds, when searched for by either
   type or location. The table form for the scam leads is also fully responsive, collapsing into an appropriate layout for devices
   as needed(including laptop and mobile). The toolbar and topbar also adjust in kind.

5. Efficiency and Accessibility:
   Analysts can take instant actions from the table without opening any detailed views. The filters and search also allow for rapid narrowing and accessibility of
   different scam leads as needed. Additionally, night mode improves readability and visibility in low-light
   environments. High contrast colours and clear labelling also further enhance the accessibility.
   
6. Error Prevention:
   The Close Case action triggers a confirmation modal with warning message, which effectively prevents accidental closure and loss of an entry/data that
   wasn't intended. Form validation prevents submission of incomplete lead information.
   
 7.  User Flow:
 The prototype supports a natural workflow, as analysts can locate leads via search or filters, quickly take appropriate actions (escalate, investigate, ignore, close),
  and view detailed information when needed. This workflow minimizes friction and ensures efficient lead management.

   
