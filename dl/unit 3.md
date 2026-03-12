![[Pasted image 20260309052033.png]]
![[Pasted image 20260309052045.png|300]]
-> weight updates happen 1 time per epoch

![[Pasted image 20260309052111.png]]
-> weight update happens m (no. of samples) time per epoch

![[Pasted image 20260309052207.png]]

best -> mini batch gradient descent

![[Pasted image 20260309052313.png]]

# Momentum

![[Pasted image 20260309052511.png]]
![[Pasted image 20260309052521.png|500]]
![[Pasted image 20260309052532.png|400]]

![[Pasted image 20260312015929.png|500]]
![[Pasted image 20260312015938.png|500]]
![[Pasted image 20260312015947.png]]
![[Pasted image 20260312124907.png]]
![[Pasted image 20260312124922.png]]

# Initialization Techniques

![[Pasted image 20260312020430.png]]
![[Pasted image 20260312020439.png]]
![[Pasted image 20260312020447.png]]

# Regularization

**L1 and L2 regularization** are techniques used in machine learning and deep learning to **prevent overfitting** by adding a penalty on large weights in the model.

They modify the **loss function** so the model prefers **smaller weights**, leading to simpler and more generalizable models.
![[Pasted image 20260312032122.png]]
![[Pasted image 20260312032223.png]]
![[Pasted image 20260312032354.png|500]]
![[Pasted image 20260312032401.png|500]]

# Learning Rate Schedules

![[Pasted image 20260312032923.png]]


$$\eta_t = \eta_{min} + \frac{1}{2}(\eta_{max}-\eta_{min})\left(1+\cos\left(\frac{t}{T}\pi\right)\right)$$

![[Pasted image 20260312104437.png]]

