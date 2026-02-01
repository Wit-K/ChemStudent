<script type="text/javascript" async
  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
</script>

# Foundations & Theory
*Part 1: The Electrochemical Basics*

---

## 1. The Big Picture
To understand this project, we must first know what electrochemical reduction is. In chemistry, "reduction" simply means gaining electrons.

Most people are familiar with combustion, where we burn a fuel with oxygen to release energy. This process produces carbon dioxide ($$CO_2$$) and water.
$$ Fuel + Oxygen \rightarrow CO_2 + H_2O + Energy $$

We can actually reverse that process and that is essentially what "CO2 Reduction (CO2R)" is. We use energy from different sources (like heat or light) to complete this process, but electrical energy is what we will be focusing on as it is the most efficient yet. Using energy to force electrons back into carbon dioxide, we can convert it from a waste product back into a useful fuel or chemical feedstock, naming it the process of "electrochemical CO2 redcution".

$$ CO_2 + H_2O + Energy (Electricity) \rightarrow Fuel + Oxygen $$

Because $$CO_2$$ is an extremely stable molecule, it does not want to react. It requires a significant amount of energy and a specific environment to break its bonds and form new ones. This is why we need an electrochemical cell.

---

## 2. Basic Electrochemistry
Experiments in this field take place inside an "electrolytic cell". Unlike a battery (which creates electricity from chemicals), an electrolytic cell uses an external power source to force non-spontaneous chemical reactions to happen.

Here are the three critical components of the system:

### The Cathode (The Reduction Site)
The cathode is the electrode connected to the negative terminal of your power supply. This is where the electrons enter the solution.
*   **What happens here:** Positive ions or neutral molecules (like $$CO_2$$) are attracted to the surface. They accept electrons and undergo reduction.
*   **Function:** This is the most important part of the setup. The material of the cathode (e.g., Copper, Gold, Silver) determines what product you make. Researchers are working together to create better cathode which makes better product.
*   **Key Equation:** $$ CO_2 + 2H^+ + 2e^- \rightarrow CO + H_2O $$

### The Anode (The Oxidation Site)
The anode is the electrode connected to the positive terminal. This is where electrons leave the solution to return to the power supply.
*   **What happens here:** To balance the electrons used at the cathode, something must lose electrons (oxidize) at the anode. In most experiments, water is oxidized into oxygen gas.
*   **Function:** While we focus on what is happening on the cathode, the anode is necessary to complete the circuit.
*   **Key Equation:** $$ 2H_2O \rightarrow O_2 + 4H^+ + 4e^- $$

### The Electrolyte
This is the liquid solution between the two electrodes. Because pure water does not conduct electricity well, we dissolve salts, like $$KHCO_3$$, (which makes the solution more conductive) into it.
*   **Function:** It allows ions to move between the cathode and anode to balance the charge. Without an electrolyte, the circuit is broken, and no reaction happens.

---

## 3. Understanding the Variables
In an electrochemical experiment, there are two main parameters we can alter or measure: Potential and Current. It is vital to understand the difference between the driving force and the reaction rate.

### Potential (Voltage)
Potential is the energy or basically, the push applied to the system. Every chemical reaction has its own minimum energy requirement to proceed.
*   **Thermodynamic Potential:** This is the theoretical minimum voltage needed to start the reaction. For converting CO2 to Carbon Monoxide, this is approximately -0.11 Volts.
*   **Applied Potential:** In the lab, you must apply significantly more voltage than the theoretical value to get the intended result. This is because real-world electrochemical reactions are hardly perfectly efficient and requires additional energy to overcome the theroretical minimum. That difference between what you apply and what is theoretically needed is called "Overpotential".

### Current (Amperage)
While voltage is the push, the current is the flow. Current measures the rate at which electrons are moving across the interface.
*   Since the chemical reaction consumes electrons, the current tells you directly how fast the reaction is happening.
*   **High Current:** A fast reaction rate.
*   **Low Current:** A slow reaction rate.

### Surface Area and Normalization
A large piece of copper will naturally allow more current to pass than a thin copper wire, just because there is more space for the reaction to occur. This makes comparision unfair. So, to make fair comparisons between different experiments, we wil look at **Current Density** instead. This is the ratio of current by surface area of the electrode telling us how active the material is regardless of its size.

---

## 4. Thermodynamics and Kinetics
A common confusion for beginners is why the reaction does not start exactly at the theoretical voltage.

### The Energy Barrier
Even if you apply enough energy to make the reaction possible (Thermodynamics), the reaction might still be too slow to measure. This is because molecules need to rearrange themselves, bonds need to break, and intermediates need to form.

### Overpotential
To overcome this slowness, we apply extra voltage. This extra voltage is the **Overpotential**.
*   If a catalyst is "good," it requires very little overpotential to reach a high current.
*   If a catalyst is "bad," you must apply a massive voltage to get even a small current.

In your research, your goal is often to find a setup that produces the most product with the least amount of overpotential (energy waste).

---

## 5. Selectivity and The Main Challenge
The most difficult part of CO2 reduction is not breaking the CO2; it is avoiding the water.

### The Hydrogen Problem
Since our electrolyte is mostly water, there are billions of water molecules surrounding the electrode for every one CO2 molecule. Water can also accept electrons to form Hydrogen gas ($H_2$).
$$ 2H^+ + 2e^- \rightarrow H_2 $$

This is called the **Hydrogen Evolution Reaction (HER)**. It is a parasitic reaction that wastes your electricity.

### Selectivity (Faradaic Efficiency)
We measure success using **Faradaic Efficiency (FE)**. This represents the percentage of electrons that went into making the product you wanted (like CO) versus the product you didn't want (like Hydrogen).
*   **100% FE:** Every electron resulted in CO2 reduction.
*   **0% FE:** All electrons were wasted making Hydrogen gas.

The choice of metal for your cathode dictates this selectivity. Some metals (like Platinum) are excellent at making Hydrogen, which makes them terrible for CO2 reduction. Other metals (like Copper, Gold, or Silver) are poor at making Hydrogen, allowing the CO2 reduction to compete effectively.
