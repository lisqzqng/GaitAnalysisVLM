# GaitAnalysisVLM
Enhancing Gait Video Analysis in Neurodegenerative Diseases by Knowledge Augmentation in Vision Language Model
## Learned Numerical Text Embedding Space
**We visualize the numerical text embeddings projected by MLPs learned through cross-modal training.** We leverage Uniform Manifold Approximation and Projection (UMAP) to reduce the embedding dimension from 64 to 3. 
* MDS-UPDRS Gait Scoring
  https://anonymous.4open.science/w/GaitAnalysisVLM-CC83/updrs.html
* Dementia subtyping
  https://anonymous.4open.science/w/GaitAnalysisVLM-CC83/diag.html
## Per-class clinical gait notions
<details>
  <summary><b>Normal</b></summary>
  Normal gait indicates normal gait without any signs of impairment. As follows are the key features and their explanations. Normal Gait Pattern: The individual walks with a normal gait pattern, which includes regular, rhythmic steps with a typical step length and height. No Shuffling or Dragging of Feet: There is no shuffling or dragging of feet while walking. Normal Arm Swing: Both arms swing naturally and symmetrically while walking, with no reduction in arm swing. No Balance Issues: The person does not have any balance problems while walking and can easily navigate turns and corners. No Assistive Device Required: There is no need for any assistive devices like a cane or walker for walking. Normal Speed and Rhythm: Walking speed and rhythm are within the normal range, and the person can easily keep pace with peers in a walking situation. No Freezing of Gait: There are no episodes of freezing of gait, where the person temporarily feels as though their feet are glued to the floor. No Difficulty with Dual Tasking: The individual can walk without difficulty while performing another task, such as talking or carrying objects.
</details>
<details>
  <summary><b>Slight</b></summary>
  Slight gait impairment indicates slight or minimal impairment in gait. It's less severe than mild gait impairment. As follows are the key features and their explanations. Minimal Impairment: The individual's walking is almost normal. Any gait abnormalities are very subtle and may not be consistently present. Occasional Slight Issues: There might be occasional problems with gait, such as a slight drag of one foot or a minimal reduction in arm swing, but these are not consistently observable. Normal Speed and Rhythm: Generally, the walking speed and rhythm are normal, and any deviations are barely noticeable. No Assistive Device Required: The person does not need any assistive device for walking, such as a cane or walker. No Falling: At this level of impairment, the individual does not have falls related to their gait. Might Be More Apparent Under Stress or Dual Tasking: Sometimes, the slight gait abnormalities may become more evident when the individual is under stress, fatigued, or while performing another task, such as talking or carrying objects.
</details>
<details>
  <summary><b>Mild</b></summary>
  Mild gait impairment definites mild impairment in gait. It's less severe than moderate gait impairment but more severe than slight gait impairment. As follows are the key features and their explanations. Mild Impairment: The impairment in walking is noticeable but not severe. The person can walk without assistance, but gait abnormalities are apparent. Possible Reduced Arm Swing: One or both arms may not swing normally while walking. There might be a reduced arm swing on one side or both sides. Slight Slowness or Shuffling: The person may walk slightly slower than normal. There might be a mild shuffling quality to the gait, but it is not pronounced. Mildly Irregular Steps: Steps might not be as regular or rhythmic as normal. There could be slight variability in step length or height. No Need for Assistive Device: Despite the mild impairment, the individual does not require a cane, walker, or any other assistive or assistant device for walking. No Falling: At this score, the person is typically not experiencing falls due to the gait impairment.
</details>
<details>
  <summary><b>Moderate</b></summary>
  Moderate gait impairment indicates moderate impairment in gait. It's more severe than mild gait impairment. As follows are the key features and their explanations. Moderate Impairment: The individual's gait is noticeably impaired, and these impairments are consistent and evident. Marked Slowness or Shuffling: The person may walk with a marked slowness. The shuffling quality of the gait can be more pronounced, with reduced step height and length. Frequent Freezing Episodes: Freezing of gait, a temporary, involuntary inability to move, may occur, especially while starting to walk or turning. Use of Assistive Devices: The individual might require a cane, walker, or other assistive devices or assistant for safe ambulation. Irregular Steps and Reduced Arm Swing: Steps may be irregular in rhythm and length, and arm swing is usually significantly reduced or absent. Possible Balance Problems: There might be issues with balance that are more apparent when walking, increasing the risk of falls. Independent Walking May Still Be Possible: Despite the moderate impairment, the person might still be able to walk independently, despite the difficulties.
</details>
* [MDS-UPDRS Gait Scoring](clinical_notions/MDS-UPDRS_Gait.txt)
* [Dementia subtyping](clinical_notions/Diagnostic_groups.txt)
## Per-class automatic prompts
* [MDS-UPDRS Gait Scoring](Automatic_prompts/MDS-UPDRS_Gait.txt)
* [Dementia subtyping](Automatic_prompts/Diagnostic_groups.txt)
