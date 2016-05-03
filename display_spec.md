# Display Specification
## at-a-glance
The feather-led display is intended to be a set of color-coded representations, skeuomorphic of LED indicators against a dark background. The base information set is defined as follows:
<table>
  <tr><th>color</th><th>measurement</th><th>semantic</th></tr>
  <tr>
    <td>green-to-yellow</td>
    <td>scalar</td>
    <td>A representation of OK-to-bogged. Usually representing response time, loading, free resources, etc. This representation implies that the measurement describes **a working system under varying intensity of load.** A green representation (rgb (0, 255, 0)) indicates nominal loading; yellow (rgb(255, 255, 0)) is the maximum loading consistent with an acceptable degree of operation. "Acceptable" is of course a figure of merit rather than a deterministic quantity.</td>
  </tr>
  <tr>
    <td>yellow-to-orange</td>
    <td>scalar</td>
    <td>A representation of bogged-to-trashed. Again, usually representing response time, loading, free resources, etc.
      This representation describes **a distressed system exhibiting varying severity of failure.**</td>
  </tr>
  <tr>
    <td colspan='2'>Obviously, for many situations the green-to-yellow and the yellow-to-orange scalars will be reasonably combined in a single measurement range. This is an alarm condition.</td>
  </tr>
  <tr>
    <td>red</td>
    <td>distinguished value</td>
    <td>The measurement cannot be obtained. This is an alarm condition.</td>
  </tr>
  <tr>
    <td>gray</td>
    <td>distinguished value</td>
    <td>Indicates an unimplemented monitoring function. Essentially, this is a placeholder in the display.</td>
  </tr>
  <tr>
    <td>purple</td>
    <td>distinguished value</td>
    <td>A configuration problem. This would be appropriate for the result of a failed consistency check on versioning of components, etc.</td>
  </tr>
</table>
