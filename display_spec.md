# Display Specification
## at-a-glance
The feather-led display is intended to be a set of color-coded representations, skeuomorphic of LED indicators against a dark background. The base information set is defined as follows:
<table>
  <tr><th>color</th><th>measurement</th><th>numeric rgb</th><th>semantic</th></tr>
  <tr>
    <td>green-to-yellow</td>
    <td>scalar</td>
    <td>(0-255, 255, 0)</td>
    <td>A representation of OK-to-bogged. Usually representing response time, loading, free resources, etc. This representation implies that the measurement describes <strong>a working system under varying intensity of load.</strong> A green representation (rgb (0, 255, 0)) indicates nominal loading; yellow (rgb(255, 255, 0)) is the maximum loading consistent with an acceptable degree of operation. "Acceptable" is of course a figure of merit rather than a deterministic quantity.</td>
  </tr>
  <tr>
    <td>yellow-to-orange</td>
    <td>scalar</td>
    <td>(255, 255-127, 0)</td>
    <td>A representation of bogged-to-trashed. Again, usually representing response time, loading, free resources, etc.
      This representation describes <strong>a distressed system exhibiting varying severity of failure.</strong> This is an alarm condition.</td>
  </tr>
  <tr>
    <td colspan='4'>Obviously, for many situations the green-to-yellow and the yellow-to-orange scalars will be reasonably combined in a single measurement range.</td>
  </tr>
  <tr>
    <td>red</td>
    <td>distinguished value</td>
    <td>(255, 0, 0)</td>
    <td>The measurement cannot be obtained. This is an alarm condition.</td>
  </tr>
  <tr>
    <td>gray</td>
    <td>distinguished value</td>
    <td>(127, 127, 127)</td>
    <td>Indicates an unimplemented monitoring function. Essentially, this is a placeholder in the display.</td>
  </tr>
  <tr>
    <td>purple</td>
    <td>distinguished value</td>
    <td>(127, 0, 255)</td>
    <td>A configuration problem. This would be appropriate for the result of a failed consistency check on versioning of components, etc.</td>
  </tr>
  <tr>
    <td>blue</td>
    <td>distinguished value</td>
    <td>(0, 0, 255)</td>
    <td>Measurement-specific failure. Used for a failure condition that cannot be generalized as slowness/burden or unavailability. This is an alarm condition.</td>
  </tr>
</table>
