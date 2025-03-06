# Fungsi untuk mengonversi suhu dari Celcius ke Fahrenheit
def celcius_to_fahrenheit(celcius):
    return (celcius * 9/5) + 32

# Fungsi untuk mengonversi suhu dari Celcius ke Kelvin
def celcius_to_kelvin(celcius):
    return celcius + 273.15

# Fungsi untuk mengonversi suhu dari Fahrenheit ke Celcius
def fahrenheit_to_celcius(fahrenheit):
    return (fahrenheit - 32) * 5/9

# Fungsi untuk mengonversi suhu dari Fahrenheit ke Kelvin
def fahrenheit_to_kelvin(fahrenheit):
    return (fahrenheit - 32) * 5/9 + 273.15

# Fungsi untuk mengonversi suhu dari Kelvin ke Celcius
def kelvin_to_celcius(kelvin):
    return kelvin - 273.15

# Fungsi untuk mengonversi suhu dari Kelvin ke Fahrenheit
def kelvin_to_fahrenheit(kelvin):
    return (kelvin - 273.15) * 9/5 + 32

# Input suhu dari pengguna
print("Pilih opsi konversi suhu:")
print("1. Celcius ke Fahrenheit")
print("2. Celcius ke Kelvin")
print("3. Fahrenheit ke Celcius")
print("4. Fahrenheit ke Kelvin")
print("5. Kelvin ke Celcius")
print("6. Kelvin ke Fahrenheit")

pilihan = int(input("Masukkan nomor pilihan (1-6): "))

suhu = float(input("Masukkan suhu: "))

if pilihan == 1:
    print(f"{suhu} Celcius = {celcius_to_fahrenheit(suhu)} Fahrenheit")
elif pilihan == 2:
    print(f"{suhu} Celcius = {celcius_to_kelvin(suhu)} Kelvin")
elif pilihan == 3:
    print(f"{suhu} Fahrenheit = {fahrenheit_to_celcius(suhu)} Celcius")
elif pilihan == 4:
    print(f"{suhu} Fahrenheit = {fahrenheit_to_kelvin(suhu)} Kelvin")
elif pilihan == 5:
    print(f"{suhu} Kelvin = {kelvin_to_celcius(suhu)} Celcius")
elif pilihan == 6:
    print(f"{suhu} Kelvin = {kelvin_to_fahrenheit(suhu)} Fahrenheit")
else:
    print("Pilihan tidak valid")
