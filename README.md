# Q-Learning in FrozenLake ❄️🏆  

## 🚀 Overview  
This project implements **Q-Learning** in the **FrozenLake environment** using [OpenAI Gym](https://gym.openai.com/).  
It demonstrates how an agent can learn to navigate a slippery frozen lake and reach the goal without falling into holes, using **reinforcement learning** techniques.  

**Highlights:**  
- ✅ **Q-learning implementation (`q_learning_frozenlake.py`)** with full training loop  
- ✅ **Dynamic image navigation (`image_navigator.py`)** for interactive diagram viewing  
- ✅ **Flowchart & FrozenLake grid images** for visual explanations  
- ✅ **Animated Q-value evolution (`Q_Learning_FrozenLake_Animation.gif`)** to see learning progress  
- ✅ **Hyperparameter tuning options** (learning rate, discount factor, exploration rate)  
- ✅ **Performance metrics visualization** with rewards and convergence plots  

---

## 📌 Q-Learning Algorithm  

Q-learning is a **model-free reinforcement learning algorithm** that learns the optimal action-selection policy using the **Bellman Optimality Equation**.  

### 🔹 Update Rule (Bellman Equation)  

\[
Q(s, a) = Q(s, a) + \alpha \Big( r + \gamma \max_{a'} Q(s', a') - Q(s, a) \Big)
\]

**Parameters:**  
- $Q(s, a)$ → Current Q-value (**expected utility of taking action $a$ in state $s$**)  
- $\alpha$ → Learning rate (**weight of new vs. old knowledge**)  
- $r$ → Immediate reward from environment  
- $\gamma$ → Discount factor (**importance of future rewards**)  
- $\max_{a'} Q(s', a')$ → Best estimated value of the next state  

**Key Concept:**  
- The agent **balances exploration vs. exploitation** using an $\epsilon$-greedy policy.  
- Over time, Q-values converge, enabling the agent to find the **optimal path** across the FrozenLake.  

---

## 📂 Project Structure  

| File | Description |
|------|-------------|
| `q_learning_frozenlake.py` | Core Q-Learning implementation with training loop |
| `image_navigator.py` | Tkinter-based interactive image viewer |
| `FrozenLake_Grid.png` | 4x4 FrozenLake board layout |
| `FrozenLake_Flowchart.png` | Step-by-step flowchart of the Q-Learning algorithm |
| `Q_Learning_FrozenLake_Animation.gif` | Animated GIF showing Q-table updates |
| `README.md` | Project documentation |

---

## ⚙️ Installation & Setup  

### 1️⃣ Install Dependencies  
Run the following command to install required libraries:  

```bash
pip install gym numpy matplotlib

### 2️⃣ Clone the Repository
git clone https://github.com/rajavigneshv/RL.git
cd RL/FrozenLake

### 3️⃣ Run Q-Learning Training
python q_learning_frozenlake.py

### 4️⃣ Run the Image Navigator
python image_navigator.py

