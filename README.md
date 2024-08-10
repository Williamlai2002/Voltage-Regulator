# Voltage-Regulator
The circuit employs an LM317 voltage regulator IC to provide a stable output voltage within the range of 3V to 3.6V. To ensure reliable operation and safeguard whatever is connected to the output from potential issues, several protective features have been integrated.


# Features
1. Regulator Output Voltage(V_out) is between 3V and 3.6V with a nominal value of 3.3V
2. The system include overvoltage protection for the output, this ensures that even when the  input voltage exceeds the maximum tolerable voltage of the LM317 which is 40V, that the output voltage is a safe voltage.
3. The system voltage includes a reverse bias protection for the input, this ensures that no components of the circuit are damaged when the polarity of the input voltage is reversed.
4. The system includes a function to stabilise output ripple to ensure that the output does not receive too much noise when a high frequency noise is added in the input. High frequency noise can be passed through the regulator to the output which may cause rippling in the output.
5. If the output is a microcontroller, the system has a function to reduce the high frequency transient noise to the regulator output introduced by the rapid on and off switching by the microcontroller. This is needed to prevent overshoots/undershoots which can damage the LM317 regulator IC or the microcontroller

# Final Design
<img width="478" alt="Screen Shot 2024-08-11 at 1 29 40 am" src="https://github.com/user-attachments/assets/9a45d42a-c9de-4935-a7b6-2f8ef0c7f4d3">
