# squared_swish
Research on the New Activation Function

Swish(Prajit Ramachandran et al.,2017) is a great discovery that effectively alleviates gradient
vanishing. Compared to ReLU(Xavier Glorot et al.,2011) piecewise linear structure, Swish curve is
more continuous and can better fit complex function mappings, especially when dealing with
high-dimensional nonlinear problems. Compared to ReLU "hard truncation" (negative input is directly
set to 0), Swish's suppression of negative signals is softer, reducing information loss. However, under
the same training configuration, Swish is convergence stability is slightly lower than ReLU. Since
Swish performs so well, is there any variant of Swish that performs better than it. So I began to explore. After extensive experimental testing, I discovered Swish's variant Squared Swish, whose formula It is f
(x)=x * sigmoid (x) * sigmoid (x), which performs better than Swish in some models.
