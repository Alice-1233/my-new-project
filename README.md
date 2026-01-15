# A simple mock-up of a risk calculation based on temperature and wind
def calculate_risk(temp, humidity, wind_speed):
    # Simplified logic: higher temp and wind + lower humidity = higher risk
    risk_score = (temp * 0.5) + (wind_speed * 0.3) - (humidity * 0.2)
    
    if risk_score > 25:
        return "HIGH RISK"
    return "LOW/MODERATE RISK"

# Example: 35°C, 10% humidity, 20km/h wind
print(f"Current conditions: {calculate_risk(35, 10, 20)}")
