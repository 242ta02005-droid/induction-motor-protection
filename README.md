# induction-motor-protection
# Induction Motor Protection System

print("===================================")
print("   INDUCTION MOTOR PROTECTION")
print("===================================")

# Safe limits
max_voltage = 250
max_current = 10
max_temperature = 80

# Get motor values
voltage = float(input("Enter Voltage (V): "))
current = float(input("Enter Current (A): "))
temperature = float(input("Enter Temperature (°C): "))

print("\nChecking Motor Conditions...")

# Protection checking
if voltage > max_voltage:
    print("⚠️ FAULT: Overvoltage detected!")
    print("🔴 Motor OFF")

elif current > max_current:
    print("⚠️ FAULT: Overcurrent detected!")
    print("🔴 Motor OFF")

elif temperature > max_temperature:
    print("⚠️ FAULT: Overtemperature detected!")
    print("🔴 Motor OFF")

else:
    print("✅ All parameters are normal")
    print("🟢 Motor ON")
    print("Motor is operating safely.")
