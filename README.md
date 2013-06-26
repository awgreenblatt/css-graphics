css-graphics
============

There are several CSS graphics-related properties that provide the bulk of support for Clipping, Masking, Filters and whatnot.  The purpose of this repo is to hopefully provide some insight into what the current state of affairs is with various browsers. 

<table>
<thead>
<tr><th>Feature</th><th>Apply To</th><th>Safari</th><th>Chrome</th><th>Firefox</th><th>IE</th><th>Opera</th><th>Comments</th></tr>
</thead>
<tbody>

<tr><td rowspan="2">clip-path with basic shapes</td><td>HTML</td><td>No</td><td>-webkit-clip-path</td><td>No</td><td>No</td><td></td><td></td></tr>
<tr><td>SVG</td><td>No</td><td>-webkit-clip-path</td><td>No</td><td>No</td><td>No</td><td></td></tr>

<tr><td rowspan="2">clip-path with SVG path</td><td>HTML</td><td>No</td><td>-webkit-clip-path</td><td>No</td><td>No</td><td></td><td></td></tr>
<tr><td>SVG</td><td>clip-path</td><td>clip-path</td><td>clip-path</td><td>clip-path</td><td>clip-path</td><td></td></tr>

<tr><td rowspan="2">mask-image</td><td>HTML</td><td>-webkit-mask-image</td><td>-webkit-mask-image</td><td>No</td><td>No</td><td></td><td>Uses alpha masking</td></tr>
<tr><td>SVG</td><td>No</td><td>No</td><td>No</td><td>No</td><td>No</td><td></td></tr>

<tr><td rowspan="2">mask-box-image</td><td>HTML</td><td>-webkit-box-image</td><td>-webkit-box-image</td><td>No</td><td>No</td><td></td><td>Uses alpha masking</td></tr>
<tr><td>SVG</td><td>No</td><td>No</td><td>No</td><td>No</td><td>No</td><td></td></tr>

<tr><td rowspan="2">mask</td><td>HTML</td><td>No</td><td>No</td><td>mask</td><td>No</td><td></td><td></td></tr>
<tr><td>SVG</td><td>mask</td><td>mask</td><td>mask</td><td>mask</td><td>mask</td><td>Uses luminance masking</td></tr>

<tr><td rowspan="2">SVG Filter</td><td>HTML</td><td>No</td><td>-webkit-filter</td><td>filter</td><td>No</td><td></td><td></td></tr>
<tr><td>SVG</td><td>filter</td><td>filter</td><td>filter</td><td>filter</td><td>filter</td><td></td></tr>
</tbody>
</table>
