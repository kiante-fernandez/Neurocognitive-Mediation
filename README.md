<h1>Using Neurocognitive Mediation Analysis to Investigate Spectral Dynamics of Evidence Accumulation Across Domains</h1>

Decisions can sometimes be classified along two dimensions: subjective versus objective criteria, and evaluation based on stimulus versus representation. Research using EEG and sequential sampling models (SSM) has provided evidence for different spatial and frequency-specific patterns of activation during choice. Yet no work has studied how EEG markers vary along these two dimensions. In our EEG study, participants made decisions in four tasks, one for each combination of dimensions. Our goals were </br>

1. to investigate which EEG markers mediate the relation between stimulus value and drift rate </br>
2. to examine whether these EEG markers differentiate between tasks. To do so, we developed a neurocognitive mediation model to jointly capture EEG, choice, and response times.</br>

<b>Keywords</b>: EEG, neurocognitive modeling, decision-making, evidence accumulation, mediation analysis
  
<h2>Background</h2>
<details>
  <summary>Definitions</summary>
  
  **Neurocognitive modeling**</br>
    In Neurocognitive modeling we seek to understand how macro-level neurophysiology (as measured by scalp-recorded EEG) encodes human cognition which gives rise to human behavior (Nunez et al., 2022). It aims to establish links between:</br>
1. brain dynamics as measured by or derived from EEG
2. cognition and other psychological concepts expressed as formal models like evidence accumulation
3. choice and response times
 
  **Mediation analysis**</br>
  The aim of Mediation analysis is to determine whether the relation between the independent variable (our experimental manipulation of stimulus difference) and the dependent variable (cognitive model parameters) is due, wholly or in part, to the mediating variable (brain dynamics) </br>
</details>

<details>
<summary>Smith et al. (2021)</summary>
Stephanie M. Smith and Ian Krajbich. Mental representations distinguish value-based decisions from perceptual decisions. Psychonomic Bulletin & Review, 28(4):1413–1422, August 2021. ISSN 1531-5320. <a href="https://link.springer.com/article/10.3758/s13423-021-01911-2">doi:10.3758/s13423-021-01911-2.</a></br>

1. Using the same set of stimuli, Smith & Krajbich experimentally study decision processes across four conditions</br>
2. They find surprisingly consistent patterns of behavior across the four decision-making conditions. The connection between stimuli differences and accuracy is very consistent. The relationship between gaze and choice is also stable across the different categories.</br>

</details>

<h2>Tasks Description</h2>

We followed a similar procedure to Smith and Krajbich (2021) with minor changes to accommodate recording EEG while subjects performed our experimental paradigm. We used a food choice paradigm that consist of two parts: pre-choice ratings, and a two alternative forced choice (2AFC) task across four categories of decisions making. The paradigm consisted of two stages: a pre-choice rating stage to elicit stimulus values for the choice task and a two-alternative forced choice (2AFC) task where participants made 100 binary choices across each of the four decision-making conditions (a total of 400 trials). Across the four decision-making conditions, subjects made decisions with the same sensory stimuli and motor outputs. Using the same stimuli with varying instructions, we could control for the differences that would prevent direct comparisons between the neural computations involved in the four simple choice paradigms. We only recorded EEG during the 2AFC task.

<details>
    <summary>Pre-choice Ratings</summary>
    In stage one, to assess different considerations people might use to make their choice, subjects first completed a pre-choice rating task. During this task, subjects rated four incentivized ratings per item, for each of 100 food images. The rating stage is blocked by the four categories of decisions making, with order randomly determined at the subject level. Subjects rated each food image on food-liking (how much they wanted to eat the food; preference-representation, PR), image size (how much space the food took up in the picture; objective-stimulus, OS), weight (how much the food weighed, relative to the other snack foods in the stimulus set; objective-representation, OR), and package (how much they liked the image; preference-stimulus, PS) (Smith and Krajbich 2021). Subjects then used the mouse to click on the rating scale. Subjects were given instructions on what the ends of the scale meant (e.g., in the food-liking category, they were told to use the left side of the scale for items that they would not like to eat and the right side of the scale for items that they would like to eat). In the PR and PS categories, ratings above/below the midpoint indicated positive/negative subjective values (i.e., liking/disliking the food or image). In the OS and OR categories, ratings above/below the midpoint indicated more/less than half of the box filled or higher/lower than average weight, respectively. 
 </details>

 <details>
    <summary>2AFC</summary>
    Then, in stage two, to assess the underlying cognitive dynamics for each class of decision making, subjects preformed the 2AFC task for each choice paradigm. For the 2AFC task, subjects made an average of 100 binary choices for each of the four decision category conditions. Every subject made choices about which of two foods they preferred to eat (PR), which of two food images they preferred (PS), which of two foods took up a greater proportion of the screen (OS), and which of two foods weighed more (OR). Subjects completed 400 total trials, split into 4 blocks of 100 trials each. Within each block there were 10 mini-blocks, each comprising 6 to 12 trials from the same condition. Thus, in total there was an average of 100 trials per condition. The exact number and order of mini-blocks was randomly determined. Item pairs were generated randomly, though subject to a few constraints. Before generating the trials, we removed options with negative subjective values in either preference category. Upon generating the trials, we limited the number of times that a food item could be seen in a condition to seven. Additionally, we limited the difference in ratings between the options to ensure that the choices are nontrivial. We used different rating-difference limits for each of the conditions, based on previous research (Smith and Krajbich 2021). </br>
    At the beginning of each trial, one of four words was presented on the screen for 1.2 second interval

1. Food liking condition: EAT
2. Weight condition: WEIGHT
3. Package condition: DESIGN
4. Image Size condition: FILL
    
To ensure that subjects followed the correct instruction, throughout each mini-block, we signaled the condition with a color code: green, yellow, red, or blue. Each color was assigned to a condition randomly at the level of the subject. The written word at the beginning of each trial and the fixation cross at the beginning of each trial were presented in the color corresponding to the condition (See Poster Figure). For each trial subjects were presented a fixation cross that remained on the screen for 0.3s and was followed by the food images. Subjects pressed one of two response keys (left arrow, or right arrow) on the keyboard to indicate their decision about which food they: preferred to eat, preferred the images for, thought took up a greater proportion of the screen, or thought weighed more. A randomly jittered 2-3 second intertrial interval separated trials following response.

</details>

<h2>Neurocognitive Mediation Analysis</h2>
We conducted a neurocognitive mediation analysis for each participant. The critical comparison in our neurocognitive mediation analysis is as follows: If the EEG markers mediated the relationship between stimulus value difference and evidence accumulation rates, the mediation model should have significant indirect effect, $\beta_{indirect_{kf}}$ , in the mediation effects controlling for a direct regression of evidence accumulation on stimulus value $\textcolor{violet}{\theta_{k}}$ .</br>
<details>
  <summary>Model Specification</summary>
 We define <em>I</em> as the pre-choice rating difference for each pair of food images. For any given trial <em>i</em> and condition  <em>k</em>, we define</br>
 
 $I_{ik} =  |r_{ImageAi} - r_{ImageBi}|$</br>

where <em>r</em> could be the rating for how much they wanted to eat the food (VD; EAT), how much space the food took up in the picture (SD; FILL), how much they liked the image (AD; DESIGN), and how much the food weighed (WD; SIZE). The model was fit for each experimental condition using random effects for each subject.</br>

To model the EEG signal for trial <em>i</em> for condition <em>k</em> we selected the first <em>f</em> principal components capturing the single-trial time-frequency representations of power and constructed the following embedded linear regression</br>

${EEG}_{ikf} \sim \mathcal{N}(\eta_{kf} + \textcolor{blue} {\beta_{kf}} \cdot I_{ik},\sigma_{noise})$</br>

$\sigma_{noise}$, describes the observation noise of the single-trial time-frequency representations of power which we assume is constant across conditions and principal components. This assumption resembles prior work by Ravenzwaaij et.al on jointly modeling of EEG data.</br>

We assume single-trial EEG measures inform single-trial DDM parameters (Nunez et al., 2017, Nunez et al., 2019).

$\delta_{ik} = \nu_{ik} + \textcolor{orange} {\gamma_{kf}} \cdot EEG_{ikf} + \textcolor{violet}{\theta_{k}} \cdot I_{ik}$</br>

These single-trial level drifts were entered into the DDM in addition to condition-level boundary separation $\alpha_{k}$ and non-decision time $\tau_{k}$ parameters (with starting point parameter $z$ fixed at 0.5).</br>

$\mathbf{y}_{ik} \sim \mathcal{W}(\delta_{ik},\alpha_{k},\tau_{k}, z)$</br>

After computing the posterior distributions we can calculate the standardized regression weights parameters $\textcolor{blue} {\beta_{kf}}$ and $\textcolor{orange} {\gamma_{kf}}$ by multiplying unstandardized weights. The indirect mediation effect, $\beta_{indirect_{kf}}$ is then calculated by multiplying the standardized regression weights, as discussed by Baron and Kenny (1986).

$\beta_{indirect_{kf}} =  (\textcolor{blue} {\beta_{kf}} \cdot \frac{\sigma_{EEG}}{\sigma_{I}})
\cdot (\textcolor{orange} {\gamma_{kf}} \cdot \frac{\sigma_{\delta}}{\sigma_{EEG}})$

</details>

<h2>References</h2>

1) Stephanie M. Smith and Ian Krajbich. Mental representations distinguish value-based decisions from perceptual decisions. Psychonomic Bulletin & Review, 28(4):1413–1422, August 2021. ISSN 1531-5320. doi:10.3758/s13423-021-01911-2.

2) Rafael Polanía, Ian Krajbich, Marcus Grueschow, and Christian C. Ruff. Neural Oscillations and Synchronization
Differentially Support Evidence Accumulation in Perceptual and Value-Based Decision Making. Neuron, 82(3):
709–720, May 2014. ISSN 0896-6273. doi:10.1016/j.neuron.2014.03.014

3) Reuben M. Baron and David A. Kenny. The moderator–mediator variable distinction in social psychological research: Conceptual, strategic, and statistical considerations. Journal of Personality and Social Psychology, 51:1173–1182, 1986. ISSN 1939-1315. doi:10.1037/0022-3514.51.6.1173.9

4) Nunez, M. D., Vandekerckhove, J., & Srinivasan, R. (2022, March 4). A tutorial on fitting joint models of M/EEG and behavior to understand cognition. https://doi.org/10.31234/osf.io/vf6t5

5) van Ravenzwaaij, D., Provost, A., and Brown, S. D. (2017). A confirmatory approach for integrating neural and behavioral data into a single model. Journal of Mathematical Psychology, 76:131–141

6) Michael D. Nunez, Joachim Vandekerckhove, and Ramesh Srinivasan. How attention influences perceptual decision making: Single-trial EEG correlates of drift-diffusion model parameters. Journal of Mathematical Psychology, 76: 117–130, February 2017. ISSN 0022-2496. doi:10.1016/j.jmp.2016.03.003.

7) Michael D. Nunez, Aishwarya Gosai, Joachim Vandekerckhove, and Ramesh Srinivasan. The latency of a visual evoked potential tracks the onset of decision making. NeuroImage, 197:93–108, August 2019. ISSN 1053-8119. doi:10.1016/j.neuroimage.2019.04.052

