## SoftMax <a name="SoftMax"></a>

**Versioned name**: *SoftMax-1*

**Category**: *Activation*

**Short description**: [Reference](https://github.com/Kulbear/deep-learning-nano-foundation/wiki/ReLU-and-Softmax-Activation-Functions#softmax)

**Detailed description**: [Reference](http://cs231n.github.io/linear-classify/#softmax)

**Attributes**

* *axis*

  * **Description**: *axis* represents the axis of which the *SoftMax* is calculated. *axis* equal 1 is a default value.
  * **Range of values**: positive integer value
  * **Type**: int
  * **Default value**: 1
  * **Required**: *no*


**Inputs**:

*   **1**: Input tensor with enough number of dimension to be compatible with *axis* attribute. Required.

**Outputs**:

*   **1**: The resulting tensor of the same shape and type as input tensor.

**Detailed description**

\f[
y_{c} = \frac{e^{Z_{c}}}{\sum_{d=1}^{C}e^{Z_{d}}}
\f]
where \f$C\f$ is a size of tensor along *axis* dimension.

**Example**

```xml
<layer ... type="SoftMax" ... >
    <data axis="1" />
    <input> ... </input>
    <output> ... </output>
</layer>
```