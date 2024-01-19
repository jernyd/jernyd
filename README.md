# Import the necessary libraries for the drill
from hardware import Drill
from hardware import MasonryBit

# Create an instance of the drill
drill = Drill()

# Create an instance of the masonry bit
masonry_bit = MasonryBit()

# Define the dimensions of the brick wall and the opening
wall_thickness = 35  # cm
opening_height = 2.089  # m
opening_width = 0.998  # m

# Calculate the position of the corner holes
corner_hole_1_x = wall_thickness / 2
corner_hole_1_y = wall_thickness / 2

corner_hole_2_x = opening_width - (wall_thickness / 2)
corner_hole_2_y = wall_thickness / 2

corner_hole_3_x = wall_thickness / 2
corner_hole_3_y = opening_height - (wall_thickness / 2)

corner_hole_4_x = opening_width - (wall_thickness / 2)
corner_hole_4_y = opening_height - (wall_thickness / 2)

# Drill the corner holes
drill.set_bit(masonry_bit)

drill.move_to(corner_hole_1_x, corner_hole_1_y)
drill.drill_hole()

drill.move_to(corner_hole_2_x, corner_hole_2_y)
drill.drill_hole()

drill.move_to(corner_hole_3_x, corner_hole_3_y)
drill.drill_hole()

drill.move_to(corner_hole_4_x, corner_hole_4_y)
drill.drill_hole()

# Cleanup
drill.turn_off()
- 👋 Hi, I’m @jernyd
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
jernyd/jernyd is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
