# GPT Hardware (gpthardware)

The goal of this project is to develop tools that enable the creation of more secure hardware.

| Method              | Description   

| Physical inspection | First, the molding coat is cut to reveal the circuitry. Then, the engineer repeatedly scans the surface while grinding the layers of the chip. There are several operations to scan the circuitry. Typical visual inspection methods are: scanning optical microscopy (SOM), scanning electron microscopy (SEM), pico-second imaging circuit analysis (PICA), voltage contrast imaging (VCI), light induced voltage alteration (LIVA) or charge induced voltage alteration (CIVA). To compare the floor plan of the chip has to be compared with the image of the actual chip. This is still quite challenging to do. To detect Trojan hardware which include (crypto) keys which are different, an image diff can be taken to reveal the different structure on the chip. The only known hardware Trojan using unique crypto keys but having the same structure is. This property enhances the undetectability of the Trojan. |

| Functional testing   | This detection method stimulates the input ports of a chip and monitors the output to detect manufacturing faults. If the logic values of the output do not match the genuine pattern, then a defect or a Trojan could be found. |
| Built-in tests       | Built-in self-test (BIST) and Design For Test (DFT) techniques add circuitry (logic) to the chip intended to help verify that the chip, as built, implements its functional specification. The extra logic monitors input stimulus and internal signals or memory states, generally by computing checksums or by exposing internal registers via a customized scanning technique. Where DFT usually coordinates with some external testing mechanism, BIST-enabled chips incorporate custom test-pattern generators. BIST functionality often exists to perform at-speed (high speed) verification where it is not possible to use scan chains or other low-speed DFT capabilities. Both methods were originally developed to detect manufacturing errors, but also have the double-edged potential to detect some effects of malicious logic on the chip, or to be exploited by malicious logic to covertly inspect remote state within the chip. |
| Side channel analyses | Every device that is electrically active emits different signals like magnetic and electric fields. Those signals – that are caused by the electric activity, can be analyzed to gain information about the state and the data which the device processes. Advanced methods to measure these side-effects have been developed and they are very sensitive (side-channel attack). Hence, it is possible to detect tightly coupled Trojans via measurement of these analog signals. The measured values can be used as a signature for the analyzed device. It is also common that a set of measured values is evaluated to avoid measurement errors or other inaccuracies. |



## We're building safer hardware.

There are various approaches to AI-based hardware trojan detection, including:

- Side-channel analysis: AI algorithms can be trained to analyze side-channel information, such as power consumption, electromagnetic emissions, or timing information, to identify potential hardware trojans.

- Layout and design analysis: Machine learning techniques can be used to examine the layout and design of integrated circuits, looking for patterns or anomalies that may indicate the presence of a hardware trojan.

- Simulation and testing: AI algorithms can be employed to simulate the behavior of electronic components under various conditions and analyze the results for indications of hardware trojans.
