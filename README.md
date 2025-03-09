# machine-learning
import numpy as np 
print ("dataset analisis de tiempo en diferentes metodos")
time = np.array([14, 23, 34], [12, 15, 7], [16, 19, 20])
print(time)
print(f"Tamaño matriz: {time.shape}")
print(f"Dimensiones: {time.ndim}")
print(f"Numero elementos: {time.size}")
print(f"primer elemento: {time[0, 0]}")
print(f"Ultimo elemento: {time[-1, -1]}")
print(f"Primera Fila: {time[0, :]}")
print(f"Ultima Columna: {time[:, -1]}")
