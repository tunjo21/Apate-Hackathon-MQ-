whats# Apate-Hackathon-MQ

## UI/UX Principles for APATE Investigation Scam Leads Portal

## Summary:
This prototype is a lightweight web-based portal designed to help fraud analysts review captured scam leads, understand and display asssociated metadata
and allow them to take appropriate investigative actions. The prototype delivers a clean UI driven by real analyst workflows, mock data for simulating real leads
and action buttons for quick remediation and triage. These actions include Escalate, Ignore and Investigate. Overall, the main focus of this prototype is to deliver an interface that is 
efficient, safe, intuitive and purpose-built for investigating scam leads.


## Applied UI/UX Principles

### 1. Clarity and Hierarchy:
   Our design aims keep the prototype clean and simple, intentionally avoiding clutter for easy display and navigation. Its minimalistic design ensures
   only essential data is displayed as required, including risk ID, scam type, the location in which it occurred and its action status. Colour coding is also used
   consistently, since each risk level is highlighted with a different colour. Status icons have other distinct colours(open - blue, ignored - grey and investigating - purple) to
   further distinguish them. Table headers are also displayed to be more larger, while rows are separated with spacing. Action buttons are grouped for quick scanning. 

### 2. Consistency:
   The interface uses one font(Montserrat) for readability and professionalism across all components. Buttons share a consistent shape
   (rounded, pill shaped for actions and rectangular for modals). Modal windows themselves follow the same layout throughout the interface: title, content
   and actions.

### 3. Status Feedback:
   The table rows and action buttons use a hover state(are raised slightly) to provide a quick and interactive response to the
   user. The models open and close clearly with smooth transitions, while the empty state prevents any confusion when there is no
   data available.

### 4. Responsiveness:
   Every icon/button has an appropriate response(light/dark switches to the mode in alternate clicks, add button adds more scam lead entries).
   The search bar near the top also allows for quick response and displays the entry in seconds, when searched for by either
   type or location. The table form for the scam leads is also fully responsive, collapsing into an appropriate layout for devices
   as needed(including laptop and mobile). The toolbar and topbar also adjust in kind.

### 5. Efficiency and Accessibility:
   Analysts can take instant actions from the table without opening any detailed views. The filters and search also allow for rapid narrowing and accessibility of
   different scam leads as needed. Additionally, night mode improves readability and visibility in low-light
   environments. High contrast colours and clear labelling also further enhance the accessibility.
   
### 6. Error Prevention:
   The Close Case action triggers a confirmation modal with warning message, which effectively prevents accidental closure and loss of an entry/data that
   wasn't intended. Form validation prevents submission of incomplete lead information.
   
### 7.  User Flow:
 The prototype supports a natural workflow, as analysts can locate leads via search or filters, quickly take appropriate actions (escalate, investigate, ignore, close),
  and view detailed information when needed. This workflow minimizes friction and ensures efficient lead management.

### 8. Risk Sorting:
      The prototype also has a feature(up and down toggle arrows) to sort the risks, their ID numbers and their ratings by ascending or descending order, so the most dangerous scam leads can be prioritised according to which
      needs to be investigated by the fraud analysts. The down arrow sorts by highest to lowest risk and risk score, while the up arrow sorts by lowest to highest risk and risk score, allowing analysts
      to prioritise the scam leads by which are the most and least urgent.
### 9. Clear Separation of Concerns:
    The different icons/buttons, such as clear fraud, clear data and add risk, are marked by red and green colors respectively, so the user has a clear view of which buttons are for adding and which are for clearing. The use of icons
    also clearly highlights the function of each button, preventing accidental usage. The status is also written in clear, all uppercase text for further clarity. The different colours for each of the buttons in
   each scam lead also highlights each's separate functionality and provides a clear demarcation of each action, providing ease of use for the user.


User Stories

User Story 1 – Lead Intake, Fraud Scan & Risk Management
As a Fraud Analyst, I want all fraud leads to appear in the portal with clear metadata, so I can immediately evaluate their severity and begin triage.
Acceptance Criteria
When the portal loads:
There are no default risks.
Analysts must add risks manually if needed.


Analyst can:
Add new risks
Delete any risk
Have zero risks if all are deleted


Analyst can create new leads through:
Scan Fraud button (manual scan)
Optional: auto-intake (if implemented)


Each new lead must include:
ID
Risk
Score
Type
Location
Status = Open


New leads appear instantly without refresh.


Long text (Type/Location/Description):
Must not overflow outside the canvas
Must use wrapping or truncation ("…")
Full content visible inside Details


Night Mode / Light Mode is available and toggles the theme.


User Story 2 – Analyst Actions & Sorting
As a Fraud Analyst, I want to take actions on each lead and sort the list so I can triage quickly and clearly.
Acceptance Criteria
Actions
Each lead has action buttons:
Escalate
Investigate
Ignore / Close ( SAME action → final )
Details


Ignore / Close Behaviour
Ignore and Close do the exact same thing:
Status changes to Closed (or Ignored— whichever wording you use)
The lead becomes final
Escalate and Investigate become disabled
Status cannot change anymore
Details
Shows all lead fields:
ID
Risk
Score
Type
Location
Description
Status
Sorting
User can sort leads by clicking column headers:
ID ascending/descending
Score ascending/descending
Risk ascending/descending


Sorting requirements:
Must toggle between ↑ and ↓
Sorting must work with filters:
e.g., “Investigating only, sorted by Score ↓”


Filtering
User can filter by:
Open
Investigating
Escalated
Closed (Ignore/Close)
Filtering:
Updates displayed leads instantly
Works with sorting



User Story 3 – Lead Outcome Tracking & Dashboard Summary
As a Team Lead, I want to understand the final states of leads so I can monitor workflow performance.
Acceptance Criteria
Dashboard displays one of these status:


Open
Investigating
Escalated
Closed (Ignore/Close)


Status persists only while the lead exists.


Counts are shown for:


Open
Investigating
Escalated
Closed


Counts update automatically when:


Status changes
Lead is closed
Lead is deleted


Sorting and filtering do not break the counts.


Escalated leads must be clearly highlighted.

