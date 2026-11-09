---
title: Research
cms_exclude: true

# Optional header image (relative to `static/media/` folder).
header:
  caption: ''
  image: ''

themes:
  - key: learning
    title: Learning-Augmented Optimization
    figure: media/research/proxy-overview.png
    caption: >-
      Offline training and online deployment of optimization proxies for order fulfillment.
    desc: >-
      Many operational problems must be solved repeatedly under tight time limits, such as
      assigning each incoming online order to a fulfillment center and carrier, or planning
      paratransit trips jointly with crew shifts. At this scale, exact solvers are often too
      slow. This line of work uses machine learning to accelerate optimization, either by
      training optimization proxies that reproduce solver decisions in real time or by using
      graph neural networks to speed up column generation.
  - key: contextual
    title: Contextual Optimization and Decision-Focused Learning
    figure: media/research/conformal-framework.png
    caption: >-
      Conformal predictive distributions turn order, fulfillment location, and carrier features into distributional forecasts of delivery time.
    desc: >-
      Operational decisions often depend on quantities that are unknown at decision time but
      partly predictable from data, such as carrier delivery times or customer choices. This
      line of work couples prediction and optimization, which are usually handled in separate
      steps. It uses conformal predictive distributions to supply calibrated uncertainty to
      stochastic and robust fulfillment models, and develops decision-focused learning
      methods that train predictive models on the cost of the decisions they induce,
      including under partial feedback and customer choice.
  - key: agentic
    title: Agentic Operations Research
    figure: media/research/reopt-llm-framework.png
    figure_width: 60%
    caption: >-
      LLM-guided re-optimization: the LLM connects the decision-maker with the optimization model, a toolbox of re-optimization techniques, and the solver.
    desc: >-
      Optimization models deployed in practice must be revised as business rules, priorities,
      and operating conditions change, and each revision usually requires a modeling expert.
      This line of work develops LLM-based agents that let decision-makers state such changes
      in natural language. The agents translate requests into structured patches to deployed
      large-scale models, select re-optimization methods to solve the updated instances, and
      elicit qualitative preferences to choose among solutions with competing objectives.
---

Selected papers are grouped by theme below. A complete list is on the [Publications](/publication/) page.
