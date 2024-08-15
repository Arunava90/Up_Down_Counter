# Up_Down_Counter
The up_down_counter module is a parameterizable counter that can count upwards or downwards based on the state of the i_up_down switch. The counter begins operation after the release of the reset signal and can be paused or resumed using single pulses on the i_pause and i_resume switches, respectively.

Up Count: The counter increments when the i_up_down switch is set to logic 1.
Down Count: The counter decrements when the i_up_down switch is set to logic 0.
Pause: When a single pulse is received on the i_pause switch, the counter pauses its operation.
Resume: The counter resumes counting when a single pulse is received on the i_resume switch.

Parameters:
COUNTER_WIDTH - Defines the bit width of the counter.

Inputs:
i_clk - Clock signal.
i_rst - Active high reset signal.
i_up_down - Controls the counting direction (1 for up, 0 for down).
i_pause - Pauses the counter on a single pulse.
i_resume - Resumes the counter on a single pulse.

Output:
o_count - The current value of the counter.

# Behavior:
The counter starts at zero after reset.
It increments or decrements based on the i_up_down input.
The counter pauses when a pulse is received on the i_pause input and resumes when a pulse is received on the i_resume input.

# Simulation Waveform:
<img width="655" alt="image" src="https://github.com/user-attachments/assets/d56fc916-16c5-4c99-9e9f-6e0573fb87c3">
<img width="710" alt="image" src="https://github.com/user-attachments/assets/9b422116-722f-4c31-a20c-e6ebb3df310a">
<img width="683" alt="image" src="https://github.com/user-attachments/assets/6cde3bb1-901d-4750-8c57-dad8b1b4d392">
