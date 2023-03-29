# Instructions

Your task is to write the code that calculates the magical energy points that get awarded to players when they complete a level.

The points awarded depend on two things:

- the number of the level that the player completed
- the base value of each magical item collected by the player during that level

There are many types of magical items, and they all have different base values.

Some examples:

- **Crystal Shard**: The Crystal Shard is a beautiful gem that glows with an ethereal light. Its base value is 2, and it is often found in underground caves.
- **Dragon Scale**: The Dragon Scale is a tough and durable material that can be used to make powerful weapons and armor. Its base value is 3, and it can be found in the lairs of ferocious dragons.
- **Phoenix Feather**: The Phoenix Feather provides warmth when days are cold and light when nights are dark. Its base value is 5, and it can be found in the nests of giant birds.
- **Mermaid Pearl**: The Mermaid Pearl is a mysterious and magical gem that is said to grant wishes. Its base value is 7, and it can be found in underwater grottos.
- **Unicorn Horn**: The Unicorn Horn is a rare and powerful item that is said to have healing properties. Its base value is 11, and it can be found in enchanted forests.

The higher the level of the player, the more items they could potentially find.

The inputs to your program are:

- the number of the level completed by the player, and
- a list of base values for the magical items collected by the player during that level.

The energy points are awarded according to the following rules:

- For each magical item, take the base value and find all the multiples of that value that are less than or equal to the level number.
- Combine the sets of numbers.
- Remove any duplicates.
- Calculate the sum of all the numbers that are left.

For example, let's say that the player completed level 20 and found two magical items with base values of 3 and 5.

To calculate the energy points earned by the player, we need to find all the unique multiples of these base values that are less than or equal to level 20.

For the base value of 3, the multiples less than or equal to 20 are: 3, 6, 9, 12, 15, 18, and 20.

For the base value of 5, the multiples less than or equal to 20 are: 5, 10, 15, and 20.

To find the unique multiples, we can combine these two sets of multiples and remove any duplicates:

{3, 5, 6, 9, 10, 12, 15, 18, 20}

The sum of all these unique multiples is:

3 + 5 + 6 + 9 + 10 + 12 + 15 + 18 + 20 = 98

Therefore, the player earns 98 energy points for completing level 20 and finding the two magical items with base values of 3 and 5.
