Download Link: https://assignmentchef.com/product/solved-syde544-assignment-5-ecg-sinus-rhythm-simulation
<br>
As we discussed during the lectures, we demonstrated that 12-lead ECG measurement is the projection of the time-varying 3-D cardiac electric vector onto the direction of each lead. A rather simple yet powerful way to simulate ECG measurements through such projection is to model the cardiac electric vector in frontal plane as a loop described by a cardioid function:

(1)

where  is a constant representing the relative size of the QRS, and  is a constant representing the sharpness of the QRS loop. Of course, the function described in Eqn. (1) has its axis laying on the x-axis, with its apex pointing towards the positive direction of the x-axis, as the dashed blue line shown in Figure 1.

<em>Figure 1 QRS Loop. The dashed line is the function in Eqn. (1), with a=4, b=1/3. And the solid line is the function rotated by  in the clock-wise direction, which is a normal QRS axis.</em>

For a normal QRS loop, a rotation to the curve has to be applied. In Figure 1, a  rotation in the clockwise direction gives a normal QRS (the solid red line).

For both P-wave and T-wave, both of which are monophasic, an elliptic model can be used:

(2)

where  and  is the length of major and minor axis of the ellipse, respectively. Again, a proper rotation needs to be applied to obtain a desired P and T loop. This is illustrated in Figure 2. (Figure 2a for P Loop and Figure 2b for T Loop).

<em>Figure 2 P and T loop. The blue dashed line are the ellipses described by Eqn. (2), and the solid red lines are the rotated loop, resulting in a normal P and T loop. The rotation angle was </em> and  respectively. <em> </em>

An overall view of the three loops (rotated) is shown in Figure 3.

<em>Figure 3 The three cardiac loops: P (blue), QRS (red) and T (black). The axis angles of the three loops is            </em>,               <em> and , respectively. </em><em> </em>

Now that we have the loops setup spatially, we need to setup the temporal sequences of the P-QRS-T sequences. For this purpose, a normal duration of the wave duration and segment, which are summarized in Table I:

<em>Table 1     The duration of the various waveforms and segments of the P-QRS-T  </em>

<table width="575">

 <tbody>

  <tr>

   <td width="115">P duration</td>

   <td width="115">PR segment</td>

   <td width="115">QRS duration</td>

   <td width="115">ST segment</td>

   <td width="115">T duration</td>

  </tr>

  <tr>

   <td width="115">110 ms</td>

   <td width="115">40 ms</td>

   <td width="115">110 ms</td>

   <td width="115">90 ms</td>

   <td width="115">150 ms</td>

  </tr>

 </tbody>

</table>




The entire waveform is illustrated in Figure 4.




<em>Figure 4 the P-QRS-T complex (by Anthony Atkielski, extracted from wikipedia).</em>

<h1>Questions</h1>

Finish the missing code in the attached script. The final script should produce a graph with the P-QRS-T wave in the six limb leads. First (left) column (from top to bottom) are I, II, and III. And the second (right) column (from top to bottom) are aVL, aVR and aVF. Please set the sampling rate at 1k Hz. This is higher than the usual ECG recordings, but should facilitate the coding.

<strong><u>Questions 1</u> </strong>

Finish the code between line 17-22, to generate QRS loop.

<strong><u>Questions 2</u> </strong>

Finish the code between line 25-30, to generate P loop.

<strong><u>Questions 3</u> </strong>

Finish the code between line 32-37, to generate T loop.

<h1>Questions 4</h1>

Finish the code between line 42-65, to generate P-QRS-T signals in the 6 limb leads. Proper annotation of the figures are required (line 52-64).