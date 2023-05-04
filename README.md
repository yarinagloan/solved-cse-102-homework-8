Download Link: https://assignmentchef.com/product/solved-cse-102-homework-8
<br>
CSE 102 –ComputerProgrammingHW 08

<table style="height: 778px;" width="1271">

 <tbody>

  <tr>

   <td width="62">91</td>

   <td width="62">92</td>

   <td width="62">T</td>

   <td width="62">94</td>

   <td width="62">95</td>

   <td width="62">96</td>

   <td width="62">97</td>

   <td width="62">S{72}</td>

   <td width="62">S{56}</td>

   <td width="62">100(Finish)</td>

  </tr>

  <tr>

   <td width="62">90</td>

   <td width="62">M{94}</td>

   <td width="62">88</td>

   <td width="62">87</td>

   <td width="62">86</td>

   <td width="62">P</td>

   <td width="62">84</td>

   <td width="62">83</td>

   <td width="62">B</td>

   <td width="62">81</td>

  </tr>

  <tr>

   <td width="62">71</td>

   <td width="62">72</td>

   <td width="62">S{68}</td>

   <td width="62">74</td>

   <td width="62">75</td>

   <td width="62">M{83}</td>

   <td width="62">77</td>

   <td width="62">78</td>

   <td width="62">T</td>

   <td width="62">80</td>

  </tr>

  <tr>

   <td width="62">70</td>

   <td width="62">M{77}</td>

   <td width="62">68</td>

   <td width="62">67</td>

   <td width="62">B</td>

   <td width="62">65</td>

   <td width="62">64</td>

   <td width="62">S{52}</td>

   <td width="62">62</td>

   <td width="62">61</td>

  </tr>

  <tr>

   <td width="62">51</td>

   <td width="62">52</td>

   <td width="62">53</td>

   <td width="62">T</td>

   <td width="62">55</td>

   <td width="62">56</td>

   <td width="62">M{77}</td>

   <td width="62">58</td>

   <td width="62">59</td>

   <td width="62">S{44}</td>

  </tr>

  <tr>

   <td width="62">B</td>

   <td width="62">49</td>

   <td width="62">P</td>

   <td width="62">47</td>

   <td width="62">46</td>

   <td width="62">S{22}</td>

   <td width="62">44</td>

   <td width="62">43</td>

   <td width="62">42</td>

   <td width="62">41</td>

  </tr>

  <tr>

   <td width="62">31</td>

   <td width="62">M{52}</td>

   <td width="62">33</td>

   <td width="62">34</td>

   <td width="62">35</td>

   <td width="62">B</td>

   <td width="62">37</td>

   <td width="62">38</td>

   <td width="62">39</td>

   <td width="62">T</td>

  </tr>

  <tr>

   <td width="62">30</td>

   <td width="62">B</td>

   <td width="62">28</td>

   <td width="62">27</td>

   <td width="62">26</td>

   <td width="62">S{12}</td>

   <td width="62">24</td>

   <td width="62">23</td>

   <td width="62">22</td>

   <td width="62">21</td>

  </tr>

  <tr>

   <td width="62">11</td>

   <td width="62">12</td>

   <td width="62">P</td>

   <td width="62">14</td>

   <td width="62">15</td>

   <td width="62">16</td>

   <td width="62">M{28}</td>

   <td width="62">18</td>

   <td width="62">19</td>

   <td width="62">20</td>

  </tr>

  <tr>

   <td width="62">10</td>

   <td width="62">9</td>

   <td width="62">8</td>

   <td width="62">M{11}</td>

   <td width="62">S{1}</td>

   <td width="62">5</td>

   <td width="62">4</td>

   <td width="62">3</td>

   <td width="62">2</td>

   <td width="62">1(Start)</td>

  </tr>

 </tbody>

</table>

Fig-1 The 100 gamesPurpose of the 100 game: Each player rolls one dice by turns and try to reach 100 block on the board as soon as possible. The player win the game who reaches 100 block firstly.Some rules of the game: Each player can roll the dice just once at his/ her turn and move forward by on the number of the dice. When a player reaches the block 100, the game is over. After the dice rolling, if the move overshoots the block 100, then the player does not move. Blocks with label “P” penalties. Similar to the first rule, if a player ends up in a “P” block after dice rolling, then the player does not move. Blocks with label “S” represents snakes. If the player reaches an “S” block, returns the block that is shown in brackets. Blocks with label “M” represents stairs. If the player reaches an “M” block, jumps the block that is shown in brackets. Blocks with label “B” represents boosts. If the player reaches a “B” block, jumps from current block to fifth next block. Blocks with label “T” represents traps. If the player reaches a “T” block, returns from current block to fifth previous block.a) Write the code of the function that initialize the board that is shown in fig-1. The board prototype should be like ;struct block board[10][10]b) Write the code of the function that prints the board like shown in fig-1. Double row cells can be printed plain (like M {11}). Don’t draw the lines which covers the blocks.c) Write the code of the function that plays the game as a single player, recursively. The function tries to reach 100. When the function reaches “100” block, it prints the moves from last to first and returns move counts.d) Write the code of the function that plays two separate game that one game for player 1 and another for player 2. Compare which player won the game and print it.Notes: Define a block named structure for blocks. The structure must have text, data, type, pos_x, pos_y, jump_x, jump_y. For example;text= M {11}data= 7type=Mpos_x=9pos_y=3block= block 11 (just represent, not the code)jump_x=8jump_y=0You can add another properties to the structure if you needed. Define an enumerated data type for block types.Part 2- Write the following recursive function:char* find_operations(int arr[], int expected_val, char operations[], size_t arr_len, int cursor, int current) 1. The first argument is an array of numbers. Assume that n numbers are given. 2. The second argument is an integer number. 3. The third argument is a string that has n-1 spaces at first call. 4. Your function finds a sequence of operators (exactly n-1 of those) such that successive application of these operators on the given array of numbers produces the given number (the second argument). The operators can be one of {+, -, *}. For example, for array {25, 12, 6, 10, 32, 8}, the operators {-, *, -, -, +} produce 44 by applying (((((25 – 12) * 6) – 10) – 32) +8). Applying the operators in sequence means that the first operator is applied to the first two numbers in the array. Assume that the result is a12. Then the second operator is applied to a12 and the third number in the array. Assume that this in turn is labeled as a123. Then the third operator will be applied to a123 and the fourth number in the array. This will continue till all the operators are applied to the numbers in the array sequentially. There may be multiple answers for the sequence of operators. You are expected to find one that works. In some cases, the given the argument may not have any n-1 operators. For example {1, 2, 3} and 100 does not have any solution. In this case, your function should return a list of spaces (n-1 of them). Notes: 1. Do not change the given function prototype. But you are allowed to use auxiliary functions as you see fit. However, your implementation of the main algorithm should be recursive. Non recursive implementations will not be graded and will receive a 0 for this part. 2. You are not allowed to use any global and static variables in your function implementations. Any use of such variables will result in a 0 for this part.