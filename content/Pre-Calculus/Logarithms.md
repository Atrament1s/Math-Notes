# Introduction
A logarithmic function is the [[Functions#Inverse Functions|inverse]] of an exponential function and can be used to solve for the exponent of an exponential function. Since logarithms are used to solve for the exponent of an exponential equation, the exponent gets isolated, the base of the exponent becomes the base of the logarithm, and the remaining number gets put in the remaining slot when converting from exponential form to logarithmic form.
$$y=a^x \leftrightarrow log_{a}(y)=x$$ ^70a85d

In a logarithm with base $a$, $\log_{a}(x)$, $a$ has the restrictions of $(a > 0, a \neq 1)$. ^417023

## Domain and Range
The domain and range of $y=a^x$ and $y=\log_{a}(x)$ are as follows. ^cf893d
<table>
	<tr>
		<th>Equation</th>
		<th>Domain</th>
		<th>Range</th>
	</tr>
	<tr>
		<td class="math display">y=a^x</td>
		<td class="math display">(-\infty,\infty)</td>
		<td class="math display">(0,\infty)</td>
	</tr>
	<tr>
		<td class="math display">y=\log_{a}(x)</td>
		<td class="math display">(0,\infty)</td>
		<td class="math display">(-\infty,\infty)</td>
	</tr>
</table>

^66a117

As can be seen, like all other inverse functions, $y=a^x$ and $y=\log_{a}(x)$'s domains and ranges are switched. ^ea424c

# Common and Natural Logarithms
The common logarithm, $\log_{10}(x)$, is commonly denoted as $\log(x)$.
The natural logarithm, $\log_{e}(x)$, is commonly denoted as $\ln(x)$. ^850334

# Rules and Properties of Logarithms
## Inverse Property
$$a^{\log_{a}(x)}=x \text{, } \log_{a}\left(a^{x}\right)=x \text{ for } a>1 \text{, } x>0$$ ^986198

This also applies to natural logarithms.
$$e^{\ln(x)}=x \text{, } \ln\left(e^{x}\right)\text{ for } x>0$$ ^d92b1f

## Product Rule
<!---AP Calculus AB A, Unit 2, Lesson 4, Page 5, Video, 10:55--->
"For any real numbers $x>0$ and $y>0$, $\log_{a} (xy)=\log_{a} (x)+\log_{a}(y)$" ^6ec43b

## Quotient Rule
$$\log_{a}\left(\frac{x}{y}\right)=\log_{a}(x)-\log_{a}(y)$$ ^53b0e7

## Power Rule
$$\log_{a}\left(x^y\right)=y\log_{a}(x)$$ ^eabacd

## Change-of-Base
In the following formula, the natural logarithm is used. This is not necessary and as long as the numerator and denominator are using the same base, any base can be used for the logarithms. It is only used as convenience as inputting the natural logarithm into a calculator usually takes less time than inputting any other logarithm.
$$\log_{a}(x)=\frac{\ln(x)}{\ln(a)}$$ ^cbe223