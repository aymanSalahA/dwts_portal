# DWTS Portal

A beautiful, organized workflow portal for managing your projects, plans, and progress.

## How to Add a New Folder

1. **Cut** your new export folder (e.g., `Chemistry_Notes`) from the `dwts_variant_1` output.
2. **Paste** it into this `dwts_portal` folder.
3. Update the portal by adding a new card (see instructions below).

## How to Update the Portal (AI Prompt)

Since this is a static site, you need to add a "Card" to `index.html` for each new folder. You can ask any AI to do this for you.

**Copy and paste this prompt to your AI:**

> "I have added a new folder named `[FOLDER_NAME]` to the `dwts_portal` directory.
> Please update `index.html` to add a new card to the grid for this folder.
> The card should follow this template (replace `FOLDER_NAME` with the actual name and customize the description and status):
>
> ```html
> <div class="card">
> 	<div class="card-header">
> 		<div class="card-title" title="FOLDER_NAME">FOLDER_NAME</div>
> 		<span class="card-badge">Active</span>
> 	</div>
> 	<div class="card-content">
> 		<p class="card-description">
> 			Brief description of this folder's purpose
> 		</p>
> 	</div>
> 	<div class="links">
> 		<a
> 			href="./FOLDER_NAME/phase_01.html"
> 			class="link-btn phase-01"
> 			target="_blank"
> 			>Phase 1</a
> 		>
> 		<a
> 			href="./FOLDER_NAME/phase_02.html"
> 			class="link-btn phase-02"
> 			target="_blank"
> 			>Phase 2</a
> 		>
> 		<a
> 			href="./FOLDER_NAME/phase_03.html"
> 			class="link-btn phase-03"
> 			target="_blank"
> 			>Phase 3</a
> 		>
> 	</div>
> </div>
> ```
>
> **Notes:**
>
> -   Replace the badge text (\"Active\") and class (\"card-badge\") with appropriate status
> -   Badge classes: `badge-secondary`, `badge-info`, `badge-success`, `badge-warning`, `badge-neutral`
> -   Update the card-description with relevant text
> -   If any phase file is missing, add the class `disabled` to that link button\""
