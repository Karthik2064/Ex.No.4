# EX.NO. 4 – EXPERIMENT 4
## GENERATE AND EVALUATE PROMPTS USING DIFFERENT PROMPT PATTERNS

**DATE:** 02-11-2026

**REGISTER NUMBER:** 212225040177

### AIM

To generate prompts using Zero-shot Prompting, Few-shot Prompting, Chain-of-Thought Prompting, Persona Pattern, Reverse Prompting, Graph Prompting, and Active Prompting, and evaluate their performance using a rubric-based evaluation method across different AI tools.

### 1. SCENARIO AND USE CASE

**Scenario: IoT-Based Smart Manufacturing Automation**

The manufacturing industry aims to improve productivity by using IoT devices, sensors, and embedded controllers. These technologies monitor machine performance, detect faults, reduce downtime, and optimize energy consumption.

**Target Audience:** Manufacturing companies in the automotive, electronics, and food-processing industries.

**Main Objectives:**

1. Improve production efficiency by 30%.
2. Minimize machinery downtime using predictive maintenance.
3. Enable real-time monitoring and remote control.
4. Reduce energy consumption through process optimization.

### 2. PROMPT PATTERNS AND EXAMPLES

#### 2.1 Zero-shot Prompting

**Definition:** Zero-shot prompting asks an AI tool to perform a task without providing examples.

**Prompt:**

"Explain how IoT sensors and embedded controllers can improve manufacturing automation. Describe real-time monitoring, predictive maintenance, energy optimization, and production efficiency in simple terms."

**Expected Output:**

IoT sensors collect machine data such as temperature, vibration, and energy consumption. Embedded controllers process sensor readings and control equipment. Predictive maintenance identifies possible failures before breakdowns occur. Real-time monitoring improves productivity and reduces downtime.

#### 2.2 Few-shot Prompting

**Definition:** Few-shot prompting provides a few examples to guide the AI in generating a similar response.

**Prompt:**

"You are designing a smart manufacturing system. Follow these examples:

Example 1:
Sensor Reading: High temperature.
Action: Generate an overheating alert.

Example 2:
Sensor Reading: Excessive vibration.
Action: Schedule machine inspection.

Now generate suitable actions for the following readings:

1. High energy consumption.
2. Low production speed.
3. Abnormal motor vibration.

Present the output in a table with columns: Sensor Reading, Possible Problem, Recommended Action."

**Expected Output:**

| Sensor Reading | Possible Problem | Recommended Action |
|---|---|---|
| High energy consumption | Inefficient operation | Check machine load and optimize energy use |
| Low production speed | Equipment malfunction | Inspect the motor and production settings |
| Abnormal motor vibration | Bearing wear or imbalance | Schedule predictive maintenance |

#### 2.3 Chain-of-Thought Prompting

**Definition:** This prompting pattern asks the AI to analyze a problem through an organized sequence of steps and provide a justified conclusion.

**Prompt:**

"Analyze a manufacturing machine that frequently stops because of overheating. Organize your response into these steps: identify the symptoms, list possible causes, determine the sensor data required, recommend a predictive maintenance solution, and explain the expected benefits. Present the main reasoning summary and final recommendations."

**Expected Output:**

1. **Symptoms:** Frequent machine stoppages and rising temperature.
2. **Possible Causes:** Poor ventilation, excessive load, or insufficient lubrication.
3. **Required Data:** Temperature, motor load, vibration, and operating time.
4. **Solution:** Install temperature and vibration sensors and analyze their readings to identify abnormal operating conditions.
5. **Expected Benefits:** Reduced unplanned downtime, improved equipment reliability, and lower maintenance costs.

#### 2.4 Persona Pattern

**Definition:** Persona prompting assigns a specific role or professional identity to the AI to obtain a response suited to that role.

**Prompt:**

"Act as an industrial IoT engineer with experience in embedded systems and smart manufacturing. Design a basic IoT-based predictive maintenance system for a manufacturing plant. Include the sensors, embedded controller, communication method, monitoring dashboard, and maintenance alerts. Explain the design in simple technical language."

**Expected Output:**

- **Sensors:** Temperature, vibration, and current sensors.
- **Controller:** ESP32 or an industrial PLC, selected according to the application.
- **Communication:** Wi-Fi, Ethernet, or an industrial communication protocol.
- **Dashboard:** Displays machine status and sensor readings in real time.
- **Alert System:** Sends notifications when readings exceed defined safety limits.
- **Maintenance:** Uses historical sensor data and suitable analytics to identify potential failures.

#### 2.5 Reverse Prompting

**Definition:** Reverse prompting starts with a desired output or solution and asks the AI to work backward to identify the requirements or prompt that could generate it.

**Prompt:**

"Desired result: A smart manufacturing system that monitors machine temperature and vibration, predicts possible failures, sends alerts, and reduces unplanned downtime.

Work backward from this desired result. Identify the required hardware, software, input data, processing steps, and implementation requirements. Finally, generate a reusable prompt that could be used to obtain a detailed system design."

**Expected Output:**

The system requires temperature and vibration sensors, an embedded controller, a communication network, a data storage system, an analytics module, and a monitoring dashboard. Historical and real-time data can be analyzed to identify abnormal conditions. The system should be tested against actual machine data before its effectiveness is evaluated.

**Generated reusable prompt:**

"Design an IoT-based predictive maintenance system for a manufacturing plant. Specify the sensors, controller, data flow, analytics, alerts, dashboard, implementation steps, and methods for measuring downtime reduction."

#### 2.6 Graph Prompting

**Definition:** Graph prompting represents relationships between system components, processes, or concepts in a graph or flowchart format.

**Prompt:**

"Create a graph-based representation of an IoT smart manufacturing system. Show the relationships among sensors, embedded controllers, the communication network, cloud or edge processing, predictive maintenance, alerts, machine control, and the monitoring dashboard. Use arrows to indicate data flow and explain the role of each component."

**Expected Output:**
~~~

<CodeBlock language="mermaid" model_previewable>
flowchart TD
    A[IoT Sensors] --> B[Embedded Controller]
    B --> C[Edge Processing]
    C --> D[Data Storage and Analytics]
    D --> E[Predictive Maintenance]
    D --> F[Monitoring Dashboard]
    E --> G[Maintenance Alerts]
    G --> H[Technician Action]
    F --> I[Remote Monitoring]
    C --> J[Machine Control]
</CodeBlock>
~~~

**Explanation:** Sensors collect machine data. The controller processes the readings and passes relevant information to the analytics system. Predictive maintenance identifies potential faults, while the dashboard and alert system help operators respond. Remote machine control must use appropriate access controls and safety interlocks.

#### 2.7 Active Prompting

**Definition:** Active prompting involves asking the AI to identify missing information or ask clarifying questions before generating a final answer.

**Prompt:**

"I want to design an IoT-based smart manufacturing system to reduce downtime and energy consumption. Before proposing the solution, ask me five important questions about the machine type, production capacity, available sensors, communication network, and budget. After receiving my answers, recommend a suitable architecture and implementation plan."

**Expected Output:**

The AI may ask:

1. What type of manufacturing equipment is used?
2. What is the current production capacity?
3. Which sensors and controllers are already available?
4. Is Wi-Fi, Ethernet, or an industrial network available?
5. What is the approximate project budget?

After receiving the answers, the AI can recommend a solution that fits the manufacturing requirements and available resources.

### 3. EVALUATION METHOD – RUBRIC-BASED EVALUATION

The prompts can be evaluated using a five-criterion rubric. Each criterion is scored from 1 to 5.

| Evaluation Criterion | Description | Maximum Marks |
|---|---|---:|
| Relevance | Addresses the manufacturing use case | 5 |
| Clarity | Instructions are understandable | 5 |
| Completeness | Covers the important requirements | 5 |
| Accuracy | Gives technically reasonable information | 5 |
| Usefulness | Provides practical and actionable output | 5 |
| **Total** | | **25** |

**Scoring Guide:**

- 5 – Excellent
- 4 – Very Good
- 3 – Good
- 2 – Needs Improvement
- 1 – Poor

### 4. COMPARISON OF DIFFERENT AI TOOLS

The same prompts can be tested using ChatGPT, Google Gemini, and Microsoft Copilot.

| Prompt Pattern | ChatGPT | Google Gemini | Microsoft Copilot |
|---|---|---|---|
| Zero-shot | Check directness and relevance | Check directness and relevance | Check directness and relevance |
| Few-shot | Check adherence to examples | Check adherence to examples | Check adherence to examples |
| Chain-of-Thought | Check stepwise summary | Check stepwise summary | Check stepwise summary |
| Persona | Check role-specific response | Check role-specific response | Check role-specific response |
| Reverse | Check backward design | Check backward design | Check backward design |
| Graph | Check graph structure | Check graph structure | Check graph structure |
| Active | Check clarifying questions | Check clarifying questions | Check clarifying questions |

**Note:** Actual scores should be entered after running the same prompts in each AI tool. The comparison table above specifies what to evaluate; it does not claim that any tool has already been tested.

### 5. SAMPLE EVALUATION RUBRIC

The following is an illustrative scoring example for one prompt. Replace these scores with the scores observed during actual testing.

| Criterion | Sample Score | Maximum |
|---|---:|---:|
| Relevance | 5 | 5 |
| Clarity | 4 | 5 |
| Completeness | 4 | 5 |
| Accuracy | 4 | 5 |
| Usefulness | 5 | 5 |
| **Total** | **22** | **25** |

**Percentage Calculation:**

Evaluation Percentage = (Total Score / Maximum Score) × 100

Sample: (22 / 25) × 100 = **88%**

### 6. PROCEDURE

1. Select the IoT-based smart manufacturing automation scenario.
2. Identify the objectives, target audience, and system requirements.
3. Write a separate prompt for each of the seven prompt patterns.
4. Submit the same prompts to the selected AI tools.
5. Collect and compare the generated responses.
6. Evaluate each response using the five-criterion rubric.
7. Calculate the total score and percentage for each response.
8. Identify which prompt pattern provides the most relevant and useful output for the selected task.

### 7. RESULT

The prompts for Zero-shot, Few-shot, Chain-of-Thought, Persona, Reverse, Graph, and Active Prompting were prepared for the IoT-based smart manufacturing automation use case. A rubric-based evaluation method and an AI tool comparison framework were established to assess the clarity, relevance, completeness, accuracy, and usefulness of the generated responses.

The final ranking of prompt patterns and AI tools can be determined after executing the prompts and recording the observed scores.
