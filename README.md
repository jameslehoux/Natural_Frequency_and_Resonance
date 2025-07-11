# Interactive Vibration Lab: A Mass-Spring-Damper Simulator

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/YOUR_USERNAME/YOUR_REPONAME/HEAD)

An interactive Jupyter Notebook for visualizing the dynamic response of a mass-spring-damper system. Use interactive sliders to adjust mass, stiffness, and damping to explore the concepts of natural frequency ($\omega_n$), damping ratio ($\zeta$), and resonance.


---

## 📚 Key Concepts

This simulation provides a hands-on tool for understanding the fundamentals of mechanical vibrations. The system's behavior is governed by the second-order differential equation:

$$ m\ddot{x} + c\dot{x} + kx = 0 $$

You can explore three critical concepts:

1.  **Natural Frequency ($\omega_n$)**: The frequency at which the system naturally oscillates without external forces. It's determined by mass and stiffness: $\omega_n = \sqrt{k/m}$.
2.  **Damping Ratio ($\zeta$)**: A dimensionless value describing how oscillations decay.
    * **$\zeta < 1$**: **Underdamped** (oscillates before settling).
    * **$\zeta = 1$**: **Critically Damped** (returns to zero as fast as possible without overshooting).
    * **$\zeta > 1$**: **Overdamped** (returns to zero slowly without oscillating).
3.  **Resonance**: The phenomenon where the vibration amplitude explodes when the driving frequency from an external force matches the system's natural frequency.

---

## 🚀 How to Use

You can run this interactive notebook in two ways: online via Binder (recommended) or locally on your own computer.

### Online (via Binder)

Click the "Launch Binder" badge at the top of this readme or use the link below. This will open a live, interactive session in your browser with no installation required.

* [**Launch Interactive Lab**](https://mybinder.org/v2/gh/YOUR_USERNAME/YOUR_REPONAME/HEAD)

### Local Installation

If you'd like to run the notebook locally, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/YOUR_REPONAME.git](https://github.com/YOUR_USERNAME/YOUR_REPONAME.git)
    cd YOUR_REPONAME
    ```

2.  **Create a virtual environment (recommended):**
    ```bash
    # For Conda
    conda create --name vibration_lab python=3.10
    conda activate vibration_lab

    # Or for venv
    python -m venv venv
    source venv/bin/activate
    ```

3.  **Install the required libraries:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Launch Jupyter Notebook:**
    ```bash
    jupyter notebook
    ```

---

## 🔬 Things to Try

Once the notebook is open, use the sliders to answer these questions:

* **Find Critical Damping:** For the default mass (m=10) and stiffness (k=1000), what value of the damping coefficient `c` makes the system critically damped ($\zeta = 1$)?
* **Observe Resonance:** Set the damping `c` to a very low value (e.g., 5.0). How does the peak of the *Frequency Response* curve change as you approach the natural frequency?
* **Effect of Mass & Stiffness:** How does doubling the mass `m` affect the natural frequency $\omega_n$? What about doubling the stiffness `k`?

---

## 💻 Technology Stack

* **Python**
* **Jupyter Notebook**
* **ipywidgets** for the interactive sliders
* **Matplotlib** for plotting
* **NumPy** & **SciPy** for numerical calculations

---

## 🤝 Contributing & Feedback

This is an educational project, and feedback is welcome! If you have suggestions for improvements or find any issues, please open an issue in the repository.
