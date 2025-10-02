# Número de materias
num_materias = int(input("¿Cuántas materias tiene el estudiante? "))

suma_promedios = 0

for i in range(num_materias):
    print(f"\nMateria {i + 1}:")
    notas = input("Introduce las notas separadas por comas (ej. 4.5, 3.0, 5.0): ")
    
    # Convertimos la cadena en una lista de floats
    lista_notas = [float(nota) for nota in notas.split(",")]
    
    # Calculamos el promedio de la materia
    promedio = sum(lista_notas) / len(lista_notas)
    print(f"Promedio de la materia {i + 1}: {promedio:.2f}")
    
    suma_promedios += promedio

print(f"\nLa suma de los promedios de todas las materias es: {suma_promedios:.2f}")
