# VLSI-NOTES
<img width="1389" height="981" alt="img1" src="https://github.com/user-attachments/assets/58efc657-cb09-4013-a09e-05f4d3754c98" />

## Full-Custom ASIC Design

In Full-Custom ASIC, all the logic cells, circuits, and layouts are designed specifically for that particular ASIC from the ground up. It is chosen **only if**:

- Existing libraries are not fast enough, or
- The logic cells are not small, or
- The power consumption is high and needs to be reduced.

### Advantages
- Delivers the **highest possible performance** at the **smallest possible die size**.

> **Die Size**: The physical dimensions, specifically the surface area, of a single, completed integrated circuit (IC) on a semiconductor wafer. It's essentially the size of the "chip" itself before it's packaged for use.

### Disadvantages
- High performance and small size come at the cost of:
  - Increased design time
  - Complex design process
  - Higher overall cost of the IC

### Examples
- Microprocessors  
- Memories  
- Analog Processors  
- Analog/Digital Communication devices  
- Sensors, Transducers  
- High-voltage ICs for automobiles

## Semi-Custom ASIC Design
## Gate Array

A **gate array** is a type of semi-custom integrated circuit (IC) containing a prefabricated array of logic gates.

### Pre-Fabricated Components
Gate arrays come with a pre-defined grid of logic gates (such as **NAND**, **NOR**, etc.) on a chip. These gates are interconnected via metal layers to create specific logic functions according to a customer’s design. It’s essentially a **partially finished chip** with pre-laid components that are later customized by adding interconnects.

In Gate Array-based ASICs:
- **P-type and N-type transistors** are pre-defined on a silicon wafer as arrays.
- Based on the customer’s logic design, **interconnections** are defined.
- The **silicon vendor** uses these to fabricate **base wafers**, which are then delivered to the customer.
- The customer-specified connections determine the final function of the chip.

---

### Types of Gate Arrays

#### 1. **Channeled Gate Array**
- Logic cells are arranged in rows.
- **Wiring channels** are provided between these rows for interconnection.
- Routing is confined to these predefined channels.
- **Summary**: Logic gates are pre-fabricated, and the interconnections are later customized using specific horizontal/vertical tracks between cells.

>  Channeled gate arrays are simpler but limited in logic density and routing flexibility.

#### 2. **Channel-less Gate Array (Sea-of-Gates)**
- Routing is performed **on top of the logic cells**, not restricted to channels.
- Also known as **Sea-of-Gates** architecture.
- Unused transistors can also be used to improve routing efficiency.
- **Advantages**:
  - Higher logic density
  - Potentially faster speeds
  - More routing flexibility

>  Channel-less gate arrays offer better performance and area efficiency at the cost of increased design complexity.

<img width="1389" height="981" alt="img2" src="Screenshot 2025-07-13 144026.png" />
