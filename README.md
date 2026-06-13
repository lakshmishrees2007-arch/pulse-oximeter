p reading at 100% maximum
if spo2 > 100:
    spo2 = 100.0

# 3. Display the results with a built-in patient safety alarm
print("\n--- Patient Vitals Report ---")
print(f"Calculated Light Ratio (R): {R:.2f}")
print(f"Blood Oxygen Saturation (SpO2): {spo2:.1f}%")

# Clinical Logic: Check for Hypoxia (low oxygen)
if spo2 >= 95:
    print("Status: NORMAL (Parint("--- Pulse Oximeter Firmware v1.0 ---")

# 1. Simulate the sensor readings (light absorption ratios)
# The device calculates a ratio 'R' between red and infrared light absorption
red_light_absorbed = float(input("Enter Red Light absorption value (e.g., 0.4): "))
ir_light_absorbed = float(input("Enter Infrared Light absorption value (e.g., 0.5): "))

# 2. BME Math: Calculate the Ratio (R)
# A lower ratio usually means more oxygenated blood
R = red_light_absorbed / ir_light_absorbed

# This is a standard linear approximation formula used in basic BME sensors
spo2 = 110 - (25 * R)

# Cap the oxygentient is well oxygenated)")
elif spo2 >= 90:
    print("Status: WARNING (Mild hypoxia - monitor closely)")
else:
    print("Status: !!! CRITICAL ALARM !!! (Severe hypoxia - provide oxygen immediately)")
