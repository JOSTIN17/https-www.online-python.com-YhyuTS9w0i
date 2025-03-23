def calcular_descuento(monto_total, porcentaje_descuento=10):
    """
    Calcula el monto del descuento aplicado a una compra.
    :param monto_total: Monto total de la compra
    :param porcentaje_descuento: Porcentaje de descuento a aplicar (por defecto 10%)
    :return: Monto del descuento
    """
    descuento = (monto_total * porcentaje_descuento) / 100
    return descuento

# Llamadas a la función
monto1 = 500
monto2 = 1000
porcentaje_personalizado = 20

descuento1 = calcular_descuento(monto1)
descuento2 = calcular_descuento(monto2, porcentaje_personalizado)

# Mostrar resultados
print(f"Compra de ${monto1}: Descuento de ${descuento1:.2f}, Monto final: ${monto1 - descuento1:.2f}")
print(f"Compra de ${monto2} con {porcentaje_personalizado}% de descuento: Descuento de ${descuento2:.2f}, Monto final: ${monto2 - descuento2:.2f}")

