print("\tWelcome to the Electrical Safety Check tool.")
print("")
print("1. Refrigerator\n2. Freezer\n3. Range (Stove)\n4. Oven (Gas or Electric)\n5. Microwave\n6. Toaster Oven\n7. Blender\n8. Food Processor\n9. Mixer\n10. Coffee Maker (Drip, Espresso, French Press, etc.)\n11. Electric Kettle\n12. Juicer\n13. Slow Cooker\n14. Rice Cooker\n15. Bread Maker\n16. Electric Grill\n17. Ice Maker\n18. Dishwasher\n19. Trash Compactor\n20. Wine Cooler\n21. Washing Machine (Top Load, Front Load)\n22. Dryer (Gas or Electric)\n23. Laundry Center (Combined Washer-Dryer)\n24. Iron\n25. Steamer\n26. Vacuum Cleaner (Upright, Canister, Handheld, Robot)\n27. Carpet Cleaner\n28. Steam Cleaner\n29. Pressure Washer\n30. Floor Polisher/Buffer\n31. Air Conditioner (Window, Portable, Split System)\n32. Heater (Space Heater, Central Heating System)\n33. Dehumidifier\n34. Humidifier\n35. Air Purifier\n36. Fan (Ceiling Fan, Floor Fan, Tower Fan)\n37. Thermostat\n38. Hair Dryer\n39. Hair Straightener/Curler\n40. Electric Shaver\n41. Electric Toothbrush\n42. Facial Cleansing Brush\n43. Massager\n44. Nail Dryer\n45. Bathroom Scale\n46. Television\n47. DVD/Blu-ray Player\n48. Home Theater System\n49. Gaming Console\n50. Streaming Device (e.g. Roku, Apple TV)\n51. Sound System/Speakers\n52. Projector\n53. Desktop Computer\n54. Laptop\n55. Printer (Inkjet, Laser)\n56. Scanner\n57. Fax Machine\n58. Shredder\n59. Paper Cutter/Trimmer\n60. Laminator\n61. Alarm Clock\n62. Electric Blanket\n63. Electric Fireplace\n64. Power Tools (Drill, Saw, Sander, etc.)\n65. Sewing Machine\n66. Smoke Detector\n67. Carbon Monoxide Detector\n68. Water Heater\n69. Water Cooler\n70. Garbage Disposal\n71. Air Fryer\n72. Sous Vide Machine\n73. Instant Pot\n74. Electric Pressure Cooker\n75. Immersion Blender\n76. Stand Mixer\n77. Food Dehydrator\n78. Espresso Machine\n79. Soda Maker\n80. Waffle Maker\n81. Pancake Griddle\n82. Electric Skillet\n83. Indoor Grill\n84. Food Steamer\n85. Electric Can Opener\n86. Spice Grinder\n87. Ice Cream Maker\n88. Yogurt Maker\n89. Popcorn Maker\n90. Electric Wine Opener\n91. Wine Aerator\n92. Wine Preserver\n93. Wine Opener\n94. Beer Fridge\n95. Beverage Cooler\n96. Soda Stream\n97. Bread Toaster\n98. Egg Cooker\n99. Crepe Maker\n100. Hot Plate\n101. Countertop Burner\n102. Electric Tea Kettle\n103. Milk Frother\n104. Electric Knife\n105. Food Slicer\n106. Food Chopper\n107. Rice Dispenser\n108. Electric Can Crusher\n109. Bagel Toaster\n110. Coffee Grinder\n111. Teapot\n112. Tea Infuser\n113. Food Scale\n114. Meat Grinder\n115. Garlic Press\n116. Citrus Juicer\n117. Margarita Machine\n118. Milkshake Maker\n119. Popcorn Popper\n120. Chocolate Fountain\n121. Fondue Pot\n122. Hot Dog Maker\n123. Tortilla Maker\n124. Quesadilla Maker\n125. Panini Press\n126. Sandwich Maker\n127. Rotisserie Oven\n128. Electric Smoker\n129. Food Warmer\n130. Buffet Server\n131. Electric Food Mill\n132. Bag Sealer\n133. Can Sealer\n134. Food Sterilizer\n135. Egg Cooker\n136. Electric Skewer\n137. Crepe Pan\n138. Omelette Maker\n139. Egg Poacher\n140. Egg Steamer\n141. Rice Warmer\n142. Sausage Maker\n143. Jerky Maker\n144. Vacuum Sealer\n145. Vacuum Chamber\n146. Jar Sealer\n147. Bottle Sealer\n148. Bag Sealer\n149. Soup Maker\n150. Chocolate Tempering Machine\n151. Exit")
appliances_info = {
    1: {"name": "Refrigerator", "max_voltage": 120, "max_current": 5, "max_resistance": 100},
    2: {"name": "Freezer", "max_voltage": 120, "max_current": 5, "max_resistance": 100},
    3: {"name": "Range (Stove)", "max_voltage": 240, "max_current": 40, "max_resistance": 50},
    4: {"name": "Oven (Gas or Electric)", "max_voltage": 240, "max_current": 30, "max_resistance": 50},
    5: {"name": "Microwave", "max_voltage": 120, "max_current": 15, "max_resistance": 20},
    6: {"name": "Toaster Oven", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    7: {"name": "Blender", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    8: {"name": "Food Processor", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    9: {"name": "Mixer", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    10: {"name": "Coffee Maker (Drip, Espresso, French Press, etc.)", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    11: {"name": "Electric Kettle", "max_voltage": 120, "max_current": 15, "max_resistance": 10},
    12: {"name": "Juicer", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    13: {"name": "Slow Cooker", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    14: {"name": "Rice Cooker", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    15: {"name": "Bread Maker", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    16: {"name": "Electric Grill", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    17: {"name": "Ice Maker", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    18: {"name": "Dishwasher", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    19: {"name": "Trash Compactor", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    20: {"name": "Wine Cooler", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    21: {"name": "Washing Machine (Top Load, Front Load)", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    22: {"name": "Dryer (Gas or Electric)", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    23: {"name": "Laundry Center (Combined Washer-Dryer)", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    24: {"name": "Iron", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    25: {"name": "Steamer", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    26: {"name": "Vacuum Cleaner (Upright, Canister, Handheld, Robot)", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    27: {"name": "Carpet Cleaner", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    28: {"name": "Steam Cleaner", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    29: {"name": "Pressure Washer", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    30: {"name": "Floor Polisher/Buffer", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    31: {"name": "Air Conditioner (Window, Portable, Split System)", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    32: {"name": "Heater (Space Heater, Central Heating System)", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    33: {"name": "Dehumidifier", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    34: {"name": "Humidifier", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    35: {"name": "Air Purifier", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    36: {"name": "Fan (Ceiling Fan, Floor Fan, Tower Fan)", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    37: {"name": "Thermostat", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    38: {"name": "Hair Dryer", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    39: {"name": "Hair Straightener/Curler", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    40: {"name": "Electric Shaver", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    41: {"name": "Electric Toothbrush", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    42: {"name": "Facial Cleansing Brush", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    43: {"name": "Massager", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    44: {"name": "Nail Dryer", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    45: {"name": "Bathroom Scale", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    46: {"name": "Television", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    47: {"name": "DVD/Blu-ray Player", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    48: {"name": "Home Theater System", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    49: {"name": "Gaming Console", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    50: {"name": "Streaming Device (e.g., Roku, Apple TV)", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    51: {"name": "Sound System/Speakers", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    52: {"name": "Projector", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    53: {"name": "Desktop Computer", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    54: {"name": "Laptop", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    55: {"name": "Printer (Inkjet, Laser)", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    56: {"name": "Scanner", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    57: {"name": "Fax Machine", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    58: {"name": "Shredder", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    59: {"name": "Paper Cutter/Trimmer", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    60: {"name": "Laminator", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    61: {"name": "Alarm Clock", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    62: {"name": "Electric Blanket", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    63: {"name": "Electric Fireplace", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    64: {"name": "Power Tools (Drill, Saw, Sander, etc.)", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    65: {"name": "Sewing Machine", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    66: {"name": "Smoke Detector", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    67: {"name": "Carbon Monoxide Detector", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    68: {"name": "Water Heater", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    69: {"name": "Water Cooler", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    70: {"name": "Garbage Disposal", "max_voltage": 120, "max_current": 10, "max_resistance": 30},
    71: {"name": "Air Fryer", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    72: {"name": "Sous Vide Machine", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    73: {"name": "Instant Pot", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    74: {"name": "Electric Pressure Cooker", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    75: {"name": "Immersion Blender", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    76: {"name": "Stand Mixer", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    77: {"name": "Food Dehydrator", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    78: {"name": "Espresso Machine", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    79: {"name": "Soda Maker", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    80: {"name": "Waffle Maker", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    81: {"name": "Pancake Griddle", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    82: {"name": "Electric Skillet", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    83: {"name": "Indoor Grill", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    84: {"name": "Food Steamer", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    85: {"name": "Electric Can Opener", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    86: {"name": "Spice Grinder", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    87: {"name": "Ice Cream Maker", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    88: {"name": "Yogurt Maker", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    89: {"name": "Popcorn Maker", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    90: {"name": "Electric Wine Opener", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    91: {"name": "Wine Aerator", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    92: {"name": "Wine Preserver", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    93: {"name": "Wine Opener", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    94: {"name": "Beer Fridge", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    95: {"name": "Beverage Cooler", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    96: {"name": "Soda Stream", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    97: {"name": "Bread Toaster", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    98: {"name": "Egg Cooker", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    99: {"name": "Crepe Maker", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    100: {"name": "Hot Plate", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    101: {"name": "Countertop Burner", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    102: {"name": "Electric Tea Kettle", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    103: {"name": "Milk Frother", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    104: {"name": "Electric Knife", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    105: {"name": "Food Slicer", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    106: {"name": "Food Chopper", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    107: {"name": "Rice Dispenser", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    108: {"name": "Electric Can Crusher", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    109: {"name": "Bagel Toaster", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    110: {"name": "Coffee Grinder", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    111: {"name": "Teapot", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    112: {"name": "Tea Infuser", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    113: {"name": "Food Scale", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    114: {"name": "Meat Grinder", "max_voltage": 120, "max_current": 10, "max_resistance": 12},
    115: {"name": "Garlic Press", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    116: {"name": "Citrus Juicer", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    117: {"name": "Margarita Machine", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    118: {"name": "Milkshake Maker", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    119: {"name": "Popcorn Popper", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    120: {"name": "Chocolate Fountain", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    121: {"name": "Fondue Pot", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    122: {"name": "Hot Dog Maker", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    123: {"name": "Tortilla Maker", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    124: {"name": "Quesadilla Maker", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    125: {"name": "Panini Press", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    126: {"name": "Sandwich Maker", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    127: {"name": "Rotisserie Oven", "max_voltage": 240, "max_current": 20, "max_resistance": 12},
    128: {"name": "Electric Smoker", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    129: {"name": "Food Warmer", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    130: {"name": "Buffet Server", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    131: {"name": "Electric Food Mill", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    132: {"name": "Bag Sealer", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    133: {"name": "Can Sealer", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    134: {"name": "Food Sterilizer", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    135: {"name": "Egg Cooker", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    136: {"name": "Electric Skewer", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    137: {"name": "Crepe Pan", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    138: {"name": "Omelette Maker", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    139: {"name": "Egg Poacher", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    140: {"name": "Egg Steamer", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    141: {"name": "Rice Warmer", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    142: {"name": "Sausage Maker", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    143: {"name": "Jerky Maker", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    144: {"name": "Vacuum Sealer", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    145: {"name": "Vacuum Chamber", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    146: {"name": "Jar Sealer", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    147: {"name": "Bottle Sealer", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    148: {"name": "Bag Sealer", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    149: {"name": "Soup Maker", "max_voltage": 120, "max_current": 5, "max_resistance": 24},
    150: {"name": "Chocolate Tempering Machine", "max_voltage": 120, "max_current": 5, "max_resistance": 24}
}
print("")
while True:
    appliance_choice = int(input("Enter the number of the appliance: "))    
    print("")
    if appliance_choice in appliances_info:
        selected_appliance = appliances_info[appliance_choice]        
        appliances_max_voltage = selected_appliance['max_voltage']
        appliances_max_current = selected_appliance['max_current']
        appliances_max_resistance = selected_appliance['max_resistance']
        print("Selected Appliance:", selected_appliance["name"])
        voltage = float(input(f"Enter your {selected_appliance['name']} voltage (in volts): "))
        current = float(input(f"Enter your {selected_appliance['name']} current (in amperes): "))
        resistance = float(input(f"Enter your {selected_appliance['name']} resistance (in ohms): ")) 
        print("")               
        if voltage > appliances_max_voltage:
            print("Voltage is too high, potential danger.")
        elif 50 <= voltage <= appliances_max_voltage:
            print("Voltage is within acceptable range.")
        elif voltage < 50:
            print("Voltage is too low, potential danger.")
        if current > appliances_max_current:
            print("Current is too high, potential danger.")
        elif 0.005 <= current <= appliances_max_current:
            print("Current is within acceptable range.")
        elif current < 0.005:
            print("Current is too low, potential danger.")
        if resistance > appliances_max_resistance:
            print("Resistance is too high, potential danger.")
        else:
            print("Resistance is within acceptable range.")
            print("")
          #Voltage  
        if voltage > appliances_max_voltage and 0.005 <= current <= appliances_max_current and resistance < appliances_max_resistance:
            print(f"Your {selected_appliance['name']} is exceeding the maximum voltage specified for it, here are some step you can take:")     
         #Current   
        if 50 <= voltage <= appliances_max_voltage and current > appliances_max_current and resistance < appliances_max_resistance:
            print(f"Your {selected_appliance['name']} is exceeding the maximum current specified for it, here are some step you can take:")   
         #Resistance   
        if voltage < 50 and current < 0.005 and resistance > appliances_max_resistance:
            print(f"Your {selected_appliance['name']} is exceeding the maximum resistance specified for it, here are some step you can take:")         
         #Voltage and Current  
        if voltage > appliances_max_voltage and current > appliances_max_current and resistance < appliances_max_resistance:
            print(f"Your {selected_appliance['name']} is exceeding the maximum voltage and current specified for it, here are some steps you can take:")
         #Current and Resistance 
        if 50 <= voltage <= appliances_max_voltage and current > appliances_max_current and resistance > appliances_max_resistance:
            print(f"Your {selected_appliance['name']} is exceeding the maximum current and resistance specified for it, here are some steps you can take:") 
        #Voltage and Resistance
        if voltage > appliances_max_voltage and 0.005 <= current <= appliances_max_current and resistance > appliances_max_resistance:
            print(f"Your {selected_appliance['name']} is exceeding the maximum voltage and resistance specified for it, here are some steps you can take:")
         #Voltage, Current and Resistance  
        if voltage > appliances_max_voltage and current > appliances_max_current and resistance > appliances_max_resistance:
            print(f"Your {selected_appliance['name']} is exceeding the maximum voltage, current and resistance specified for it, here are some steps you can take:")
    else:
             print("Exiting Program")
             break
             
            
            
           
        
        
        
        
