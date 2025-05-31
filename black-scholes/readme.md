# Understanding Black - Scholes Forumla
European Call Option:
> European call options can only be **exercised at expiration** (one time), unlike American options which can be **exercised at any time** before expiration.
$$
\\
\\
\textbf{Variables:}
\\
C_0 = European\ Call\ Option\ Price
\\
S_0 = Current\ Stock\ Price
\\
X = Exercise\ Price
\\
r = Risk\ Free\ Interest\ Rate
\\
T = Time\ to\ Expiration
\\
\sigma = Volatility\ of\ the\ Stock\ (standard\ deviation\ of\ log\ returns)
\\
|-------------|
\\
\textbf{European Call Option:}
\\
C_0 = S_0\,N(d_1) - X e^{-rT}\, N(d_2)
\\
|-------------|
\\
Where:

\quad
d_{1,2} = \frac{\ln(S_0/X) + (r\pm\tfrac12\sigma^2)T}{\sigma\sqrt{T}}
$$ 

## Relative terms:

* **Higher current stock price** (comapred to exercise price) = higher chance of exercising the option = **higher price of the option**

* **Lower exercise price** (compared to current stock price) = higher chance of exercising the option = **higher price of the option**

* **Volatility** = More volatile the stock, more likely it is to reach the exercise price = **higher price of the option**
* * $$ \sigma\ goes\ up\ \Rightarrow\ d_1 \ goes\ up\ \Rightarrow\ d_2 \ goes \ down \Rightarrow\ \ C_0 \ goes\ up $$
---

**Example:**
If stock price is $100, and excercise price is $50.
$$
C_0 = 100 * N(d1) - 50 * e^{-rT} * N(d2)
$$
Inside the N(d1) and N(d2) functions, the proportionality would be higher, leading to a higher option price:
$$
\frac{Current\ Stock\ Price}{Exercise\ Price} = \frac{S_0}{X} = \frac{100}{50} = 2
$$







