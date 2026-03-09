import requests
ip = input("Enter an IP address: ")

url = f"http://ip-api.com/json/{ip}"

response = requests.get(url)

data = response.json()

print("IP:", data["query"])

print("Country:", data["country"])

print("City:", data["city"])

print("ISP:", data["isp"])

print("Latitude:", data["lat"])

print("Longitude:", data["lon"])

print("Timezone:", data["timezone"])

print("AS:", data["as"])
print("Organization:", data["org"])

