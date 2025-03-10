# machine-learning
import numpy as np 
print ("dataset analisis de tiempo en diferentes metodos")
time = np.array ([[14, 23, 34], [12, 15, 7], [16, 19, 20]])
print(time)
print(f"Tamaño matriz: {time.shape}")
print(f"Dimensiones: {time.ndim}")
print(f"Numero elementos: {time.size}")
print(f"primer elemento: {time[0, 0]}")
print(f"Ultimo elemento: {time[-1, -1]}")
print(f"Primera Fila: {time[0, :]}")
print(f"Ultima Columna: {time[:, -1]}")
# Promedio
prom = np.mean(time)
print("El promedio de los tiempos es:", prom)

# Desviacion Estandar
devstd = np.std(time)
print(f"La desviacion estandar de los tiempos es: {devstd:.2f}")

# Promedio por metodo
metodoA = np.array([14, 23, 34])
metodoB = np.array([12, 15, 7])
metodoC = np.array([16, 19, 20])

promA = np.mean(metodoA)
promB = np.mean(metodoB)
promC = np.mean(metodoC)
print(f"Promedio de A: {promA}, Promedio de B {promB}, Promedio de C: {promC}")

# Desviacion por Metodo
desvA = np.std(metodoA)
desvB = np.std(metodoB)
desvC = np.std(metodoC)
print(f"Desv_Estandar de A: {desvA:.2f}, Desv_Estandar de B: {desvB:.2f}, Desv_Estandar de C: {desvC:.2f}")

#Mediana
mediana = np.median(time)
print(f"La mediana de los tiempos es: {mediana}")

#Varianza
varianza = np.var(time)
print(f"La varianza de los tiempos es: {varianza:.2f}")

#Percentiles
percentil = np.percentile(time, 50)
print(f"El percentil 50 de los tiempos es: {percentil}")

#Máximo
maximo = np.max(time)
print(f"El valor maximo de los tiempos es: {maximo}")

#Mínimo
minimo = np.min(time)
print(f"El valor minimo de los tiempos es: {minimo}")

#Rango
rango = np.max(time) - np.min(time)
print(f"El rango de los tiempos es: {rango}")

#suma
suma = np.sum(time)
print(f"La suma de los tiempos es: {suma}")

#Producto
producto = np.prod(time)
print(f"El producto de los tiempos es: {producto}")

#Suma por filas y columnas
suma_filas = np.sum(time, axis=0)
suma_columnas = np.sum(time, axis=1)
print("Suma por filas:", suma_filas)
print("Suma por columnas:", suma_columnas)

#Matriz transpuesta
transpuesta = np.transpose(time)
print("Matriz transpuesta:")
print(transpuesta)

#Determinante
determinante = np.linalg.det(time)
print("Determinante de la matriz:")
print(determinante)
