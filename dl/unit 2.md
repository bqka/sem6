---
share_link: https://share.note.sx/d0vr0taj#xRigqY/3aXweCbCi+FdtDDN/CdufBz3ECPdWnN6nW7s
share_updated: 2026-05-14T22:57:29+05:30
---
# Activation Functions

![[Pasted image 20260309034857.png|500]]
![[Pasted image 20260309034910.png|500]]
![[Pasted image 20260309034922.png|400]]
![[Pasted image 20260309034939.png|400]]
![[Pasted image 20260309035015.png|500]]

# Gradient Problems

![[Pasted image 20260309035408.png]]
![[Pasted image 20260309035450.png]]
![[Pasted image 20260309035506.png]]
![[Pasted image 20260309035552.png]]
![[Pasted image 20260309035603.png]]

# Normalization

![[Pasted image 20260312024404.png]]
![[Pasted image 20260312024723.png]]
![[Pasted image 20260312033252.png]]

![[Pasted image 20260515023507.png]]


![[Pasted image 20260312024817.png]]

# Receptive Field

The **receptive field** of a neuron in a CNN is:
> the region of the original input image that can influence that neuron’s output.

```
new RF = old RF + (kernel−1) × total stride so far
update stride = old stride x curr layer stride
```
![[Pasted image 20260515102844.png]]

# Gradient Clipping

![[Pasted image 20260312031725.png]]
if |gradient| > threshold  
gradient = threshold
![[Pasted image 20260312032002.png]]