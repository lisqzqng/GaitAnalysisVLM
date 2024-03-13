# GaitAnalysisVLM
Enhancing Gait Video Analysis in Neurodegenerative Diseases by Knowledge Augmentation in Vision Language Model
## Learned Numerical Text Embedding Space
**We visualize the numerical text embeddings projected by MLPs learned through cross-modal training.** We leverage Uniform Manifold Approximation and Projection (UMAP) to reduce the embedding dimension from 64 to 3. 
* <a href="https://anonymous.4open.science/w/GaitAnalysisVLM-CC83/updrs.html" target="_blank">MDS-UPDRS Gait Scoring</a>

<img>
  <iframe id="inlineUPDRS" title="inlineUPDRS" width="300" height="300" src="https://anonymous.4open.science/w/GaitAnalysisVLM-CC83/updrs.html"></iframe>
</img>

* <a href="https://anonymous.4open.science/w/GaitAnalysisVLM-CC83/diag.html" target="_blank">Dementia subtyping</a>
  
## Per-class clinical gait notions
We employ specific clinical gait notions to develop per-class learnable prompts for prompt tuning. These notions have been generated using ChatGPT-4, then subsequently filtered, modified, and validated by a neurologist.

* **MDS-UPDRS Gait Scoring**
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

* **Dementia subtyping**
  <details>
  <summary><b>Healthy</b></summary>
  Normal gait has the following features. Stability: healthy individuals usually have stable gait patterns with consistent stride lengths and minimal sway. Stride Length: healthy individuals tend to have longer stride lengths than in DLB and AD. Cadence: healthy people maintain a regular and consistent cadence. Speed: walking speed is generally faster and more consistent than in DLB and AD. Symmetry: gait is symmetrical with even distribution of weight and movement. Rhythm: rhythm of walking is consistent, with predictable heel-to-toe sequences. Arm Swing: there is natural arm swing in synchronisation with leg movements.
  </details>
  
  <details>
  <summary><b>Dementia with Lewy Bodies</b></summary>
  Gait in Dementia with Lewy Bodies (DLB) has the following features. Slowness: markedly slower walking speed compared to healthy individuals, and more marked slowness than in AD. Postural Instability: difficulty in maintaining upright posture. Rigidity: stiffness in movement, which can affect the fluidity of the gait. Freezing of gait: the feet feel as if they are stuck to the floor. Shuffling: tendency to shuffle feet, with reduced lift-off, which increases the risk of tripping and resembles Parkinsonian gait. Reduced arm swing: can be more pronounced than in AD. Balance problems: more pronounced balance problems than in AD and falls are more frequent than in AD.
  </details>
  
  <details>
  <summary><b>Alzheimer's Disease</b></summary>
  Gait in Alzheimer's Disease (AD) has the following features. Slowness: similar to DLB, individuals with AD may walk more slowly than healthy individuals. Dual-task Difficulty: greater difficulty walking while performing another task than in DLB, leading to more pronounced gait disturbances when talking. Cadence: The cadence may become irregular, contributing to an overall unsteady gait. Postural Instability: individuals with AD may have difficulties with balance and posture but it’s less pronounced than in DLB. AD primarily shows a decline in spatial navigation and executive function, affecting gait indirectly through cognitive decline rather than direct motor impairment.
  </details>


## Per-class automatic prompts
We extract keywords from clinical gait notions to make per-class automatic prompts.

* **MDS-UPDRS Gait Scoring**
  <details>
  <summary><b>Normal</b></summary>
  Normal Gait Pattern, No Shuffling or Dragging of Feet, Normal Arm Swing, No Balance Issues, No Assistive Device or assistant Required, Normal Speed and Rhythm, No Falling, No Freezing of Gait, No Difficulty when performing Dual Tasking.  
  </details>
  
  <details>
  <summary><b>Slight</b></summary>
  Any gait abnormalities are very subtle and may not be consistently present, Occasional Slight Issues, Normal Speed and Rhythm, No Assistive Device or assistant Required, No Falling, Might Be More Apparent when performing Dual Tasking. 
  </details>
  
  <details>
  <summary><b>Mild</b></summary>
  Impairment in walking is noticeable but not severe, Possible Reduced Arm Swing, Slight Slowness or Shuffling, Irregular Steps, No Need for Assistive Device or assistant, No Falling.
  </details>
  
  <details>
  <summary><b>Moderate</b></summary>
  Gait is noticeably impaired and impairments are consistent and evident, Marked Slowness or Shuffling, Frequent Freezing Episodes, Assistance device or from others required, Irregular Steps and Reduced Arm Swing, Possible Balance Problems, may still possible to walk alone. 
  </details>

* **Dementia subtyping**
  <details>
  <summary><b>Healthy</b></summary>
  consistent stride length and minimal sway, regular and consistent cadence, fast and consistent walking speed, symmetrical gait with even distribution of weight and movement, consistent rhythm, natural arm swing in synchronisation with leg movements
  </details>
  
  <details>
  <summary><b>Dementia with Lewy Bodies</b></summary>
  slowness, evident postural instability, stiffness in movement, rigidity, Freezing of gait, shuffle feet with reduced lift-off, pronounced balance problems, irregular cadence, reduced arm swing, high risk of falls
  </details>
  
  <details>
  <summary><b>Alzheimer's Disease</b></summary>
  slowed walking speed, difficulty walking while speaking, irregular cadence, postural instability, balance problem, decline in spatial navigation, risk of falls
  </details>

