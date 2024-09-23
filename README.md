# Pr-en-clase-km-litros-motocicleta
Alvaro Campechano Estrada 3W

print(" ")
print("Alvaro Campechano practica en clase que solicite al usuario ingresar la cantidad de kilómetros recorridos por una motocicleta y la cantidad de litros de combustible que consumió durante ese recorrido.")
print(" ")
# Programa para calcular el consumo de combustible de una motocicleta

def calcular_consumo_por_km(kilometros, litros):
    """
    Función que calcula el consumo de combustible por kilómetro.
    
    Parámetros:
    kilometros (float): La cantidad de kilómetros recorridos.
    litros (float): La cantidad de litros de combustible consumidos.
    
    Retorna:
    float: Consumo de combustible por kilómetro.
    """
    if kilometros <= 0:
        raise ValueError("La cantidad de kilómetros debe ser mayor que cero.")
    if litros < 0:
        raise ValueError("La cantidad de litros no puede ser negativa.")
    
    return litros / kilometros

def main():
    # Solicitar al usuario la cantidad de kilómetros recorridos
    try:
        kilometros = float(input("Ingrese la cantidad de kilómetros recorridos: "))
        # Solicitar al usuario la cantidad de litros de combustible consumidos
        litros = float(input("Ingrese la cantidad de litros de combustible consumidos: "))
        
        # Calcular el consumo de combustible por kilómetro
        consumo_por_km = calcular_consumo_por_km(kilometros, litros)
        
        # Mostrar el resultado
        print(f"El consumo de combustible por kilómetro es: {consumo_por_km:.2f} litros/km")
    
    except ValueError as e:
        print(f"Error: {e}")

# Ejecutar el programa
if __name__ == "__main__":
    main()

![image](https://github.com/user-attachments/assets/af5087b8-a3a3-4a4d-9be6-7f145f04ddc2)
![image](https://github.com/user-attachments/assets/cb7173b8-ef5b-4f18-a8c8-5284f317143a)


