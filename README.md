# EWMA-Decay-f-for-Power-bi
ACWR (SMA, EWMA 3/21 days, EWMA 7/28 days) with decay factor for days…
The script is gethering data from one (Google sheet) source. 
One code calculate SMA and EWMA without decay factor. The other one with decay factor. 
Bought codes, output data in two separate Google sheet. After that you can connect those two Gdrive Sheet with Power bi for visualisation purposes... 

About decay factor
ACWR with a Decay Factor is generally more realistic for following the training load over time. It better represents the athlete's true workload by smoothing out the transitions between training and rest days, leading to more stable and actionable ACWR ratios. If your goal is to maintain athletes within the optimal workload range and avoid sudden spikes or dips in the ACWR, using a decay factor will provide a more accurate and reliable measure. This will help you better manage training loads and reduce the risk of injury or under-training.

Using a decay factor in the 5-10% range per day without training is recommended. This range strikes a balance between accurately reflecting the ongoing influence of past training loads while allowing the ACWR to adapt as the athlete recovers. A 5% decay is more conservative, making it suitable for athletes with longer recovery periods or who want to maintain a higher influence of past training sessions. On the other hand, a 10% decay, which this model uses, is more aggressive and is better suited for athletes with shorter recovery periods or when you need the ACWR to react more quickly to changes in training load. (You can adjust this range depending on the specific needs of your athletes, their recovery rates, and your monitoring goals.)

Using a decay factor will help maintain the integrity of the Acute Workload Ratio (ACWR). Here's how it will affect your ACWR ratios:

Impact on ACWR (EWMA3/EWMA21 and EWMA7/EWMA28):

Maintained Continuity:
The decay factor ensures that training load does not drop to zero on rest days, allowing your ACWR to reflect a more continuous and realistic load progression. This is crucial for avoiding sharp dips in the ratio that could misrepresent the athlete's true workload and risk.

Smoother Ratios:
Because the decay factor only slightly reduces the training load each day (e.g., 5-10%), your EWMA3 and EWMA7 will decrease gradually over rest days. This means that the short-term average will not suddenly plummet, which could otherwise cause the ACWR to spike or drop unnaturally.

Alignment with Recommendations:

With the decay factor, your ACWR is more likely to stay within the recommended ranges:

< 0.80: With a decay factor, you're less likely to see abrupt drops that push your ACWR below this threshold unless there are extended periods without training.
0.80 – 1.30: The decay factor helps keep the ratio in this optimal range, as the short-term load will decrease more gently, aligning well with the longer-term chronic load.
> 1.50: This zone is the "danger zone," which would typically occur if the short-term load sharply increases relative to the chronic load. The decay factor reduces the likelihood of this happening suddenly due to short rest periods, as it tempers the short-term load.
