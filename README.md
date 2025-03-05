# Q-Learning in FrozenLake ❄️🏆

## 🚀 Overview
This project implements **Q-Learning** in the **FrozenLake environment** using OpenAI Gym.  
It demonstrates how an agent can learn to navigate a frozen lake safely using **reinforcement learning**.

**Features:**
- ✅ **Q-learning implementation (`q_learning_frozenlake.py`)**  
- ✅ **Dynamic image navigation (`image_navigator.py`)** to view diagrams interactively.  
- ✅ **Flowchart & FrozenLake grid images** for clear explanations.  
- ✅ **Animated Q-value evolution (`Q_Learning_FrozenLake_Animation.gif`)** showing how learning improves over time.  

---

## 📌 **Q-Learning Algorithm**
Q-learning is a **model-free reinforcement learning algorithm** that learns the optimal action-selection policy.

### **🔹 Bellman Equation (Q-Value Update Rule)**

Q(s, a) = Q(s, a) + \alpha \left( r + \gamma \max_{a{\prime}} Q(s{\prime}, a{\prime}) - Q(s, a) \right)


Where:
	•	 Q(s, a)  → Current Q-value (how good is taking action  a  in state  s )
	•	 \alpha  → Learning rate (controls how much new values influence updates)
	•	 r  → Immediate reward (reward received after taking action  a  in state  s )
	•	 \gamma  → Discount factor (determines how much future rewards matter)
	•	 \max_{a{\prime}} Q(s{\prime}, a{\prime})  → Best possible Q-value from the next state  s{\prime} 
(assuming the agent chooses the optimal action  a{\prime}  in state  s{\prime} )

**Key Idea:**  
- The agent **balances immediate rewards** and **long-term future rewards** to make better decisions over time.  
- As it plays more episodes, **Q-values converge to the optimal policy**.

---

## 📂 **Files Included**
| File | Description |
|------|------------|
| `q_learning_frozenlake.py` | Q-Learning implementation in OpenAI Gym |
| `image_navigator.py` | Tkinter-based image viewer for diagrams |
| `FrozenLake_Grid.png` | 4x4 FrozenLake grid representation |
| `FrozenLake_Flowchart.png` | Q-learning algorithm flowchart |
| `Q_Learning_FrozenLake_Animation.gif` | Animation showing Q-value updates |
| `README.md` | Project Documentation |

---

## 📌 **How to Run the Project**
### **1️⃣ Install Dependencies**
Run the following command to install required libraries:

```sh
pip install gym numpy matplotlib tkinter
