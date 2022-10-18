```mermaid
  journey
    title Data Breach Report (Full Journey)
    section Initial Submission
      Open form and make report: 3: Submitter
    section Initial Assessment
      Open form and read report: 3: DPM
      Determine more information required: 2: DPM
	  Return to submitter for more information: 3: DPM, System
	section Additional Information
	  View response from Data Protection Team: 3: Submitter
	  Open form with existing data: 3: Submitter
	  Add requested information: 3: Submitter
	  Submit new version of form: 3: Submitter
	section Reassess
	  Open new version of form: 3: DPM
	  Determine need to assemble Data Breach Panel (DBP): 1: DPM
	  Create private teams channel: 3: System
	  Identify and notify panel members: 2: DPM, System
	section DBP Meet
	  Assess form: 3: DBP
	  Determine need to submit to ICO: 1: DBP
	  Generate report for ICO: 2: DPM, System
	section ICO assessment
	  Assess report: 3: ICO
	  Await reponse and liaise with ICO: 3: DPM
	  Return Response: 3: ICO
	section Close Case
	  Implement ICO recommendations: 4: DPO, DPM
	  Close Case: 5: DPM
```