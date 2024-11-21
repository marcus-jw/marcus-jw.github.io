---
layout: home
---

<div class="profile-section">
  <img src="{{ site.baseurl }}/assets/images/marcus.jpg" alt="Marcus Williams" class="profile-image">
  <div class="profile-text">
    <h1>Marcus Williams</h1>
    <p>I am an AI safety researcher currently investigating targeted deception in LLMs at MATS. I am also working on a project on chain of thought faithfulness and out-of-context reasoning. My previous work has involved improving preference modeling for scalable oversight and formally proving the expressivity relationships between alternative RL formalisms.</p>
  </div>
</div>

## Latest Publications

<ul>
  <li>
    <a href="https://arxiv.org/abs/2411.02306">On Targeted Manipulation and Deception when Optimizing LLMs for User Feedback</a> (Oral at SATA, spotlight at SoLaR, submitted to ICLR 2025)
    <details>
      <summary>Abstract</summary>
      As LLMs become more widely deployed, there is increasing interest in directly optimizing for feedback from end users (e.g. thumbs up) in addition to feedback from paid annotators. However, training to maximize human feedback creates a perverse incentive structure for the AI to resort to manipulative or deceptive tactics to obtain positive feedback from users who are vulnerable to such strategies. We study this phenomenon by training LLMs with Reinforcement Learning with simulated user feedback in environments of practical LLM usage. In our settings, we find that:
      <ol>
        <li>Extreme forms of ``feedback gaming'' such as manipulation and deception are learned reliably</li>
        <li>Even if only $2\%$ of users are vulnerable to manipulative strategies, LLMs learn to identify and target them while behaving appropriately with other users, making such behaviors harder to detect</li>
        <li>To mitigate this issue, it may seem promising to leverage continued safety training or LLM-as-judges during training to filter problematic outputs. Instead, we found that while such approaches help in some of our settings, they backfire in others, sometimes even leading to subtler manipulative behaviors.</li>
      </ol>
      We hope our results can serve as a case study which highlights the risks of using gameable feedback sources, such as user feedback, as a target for RL.
    </details>
    <div class="repo-link">
      [<a href="https://github.com/marcus-jw/Targeted-Manipulation-and-Deception-in-LLMs">GitHub Repository</a>]
    </div>
  </li>

  <li>
    <a href="https://arxiv.org/abs/2310.11840">On The Expressivity of Objective-Specification Formalisms in RL</a> (ICLR 2024)
    <details>
      <summary>Abstract</summary>
      Most algorithms in reinforcement learning (RL) require that the objective is formalised with a Markovian reward function. However, it is well-known that certain tasks cannot be expressed by means of an objective in the Markov rewards formalism, motivating the study of alternative objective-specification formalisms in RL such as Linear Temporal Logic and Multi-Objective Reinforcement Learning. To date, there has not yet been any thorough analysis of how these formalisms relate to each other in terms of their expressivity. We fill this gap in the existing literature by providing a comprehensive comparison of 17 salient objective-specification formalisms. We place these formalisms in a preorder based on their expressive power, and present this preorder as a Hasse diagram. We find a variety of limitations for the different formalisms, and argue that no formalism is both dominantly expressive and straightforward to optimise with current techniques. For example, we prove that each of Regularised RL, (Outer) Nonlinear Markov Rewards, Reward Machines, Linear Temporal Logic, and Limit Average Rewards can express a task that the others cannot. The significance of our results is twofold. First, we identify important expressivity limitations to consider when specifying objectives for policy optimization. Second, our results highlight the need for future research which adapts reward learning to work with a greater variety of formalisms, since many existing reward learning methods assume that the desired objective takes a Markovian form. Our work contributes towards a more cohesive understanding of the costs and benefits of different RL objective-specification formalisms. 
    </details>
  </li>

  <li>
    <a href="https://arxiv.org/abs/2406.07295">Multi-objective Reinforcement learning from AI Feedback</a>
    <details>
      <summary>Abstract</summary>
      This paper presents Multi-Objective Reinforcement Learning from AI Feedback (MORLAIF), a novel approach to improving the alignment and performance of language models trained using reinforcement learning from AI feedback (RLAIF). In contrast to standard approaches that train a single preference model to represent all human preferences, MORLAIF decomposes this task into multiple simpler principles, such as toxicity, factuality, and sycophancy. Separate preference models are trained for each principle using feedback from GPT-3.5-Turbo. These preference model scores are then combined using different scalarization functions to provide a reward signal for Proximal Policy Optimization (PPO) training of the target language model. Our experiments indicate that MORLAIF outperforms the standard RLAIF baselines and that MORLAIF can be used to align larger language models using smaller ones. Surprisingly, the choice of scalarization function does not appear to significantly impact the results. 
    </details>
    <div class="repo-link">
      [<a href="https://github.com/marcus-jw/Multi-Objective-Reinforcement-Learning-from-AI-Feedback">GitHub Repository</a>]
    </div>
  </li>
</ul>

[View my full CV](/cv/)
