css-graphics
============

There are several CSS graphics-related properties that provide the bulk of support for Clipping, Masking, Filters and whatnot.  The purpose of this repo is to hopefully provide some insight into what the current state of affairs is with various browser implementations.

The 'Apply To' column below distinguishes whether we're talking about applying the feature to HTML or SVG graphic components.  If you apply a feature to an entire embedded SVG graph, that falls under the HTML category.  If however, you're talking about applying the feature to a subgraph within the SVG, that falls into the SVG category.

For each browser column, a 'No' indicates the feature is currently unsupported.  Otherwise, I indicate whether the feature is currently vendor-prefixed or not.

I don't have much information at this point on Opera, so have decided to leave it out for now.  If you want, go ahead and fill it out and do a pull request.

In fact, if any of this information is out of date or incomplete, please update and do a pull request.

<table>
<thead>
<tr><th>Feature</th><th>Apply To</th><th>Safari</th><th>Chrome</th><th>Firefox</th><th>IE</th><th>Comments</th></tr>
</thead>
<tbody>

<tr><td rowspan="2"><a href="http://docs.webplatform.org/wiki/css/properties/clip-path">clip-path</a> with basic shapes</td><td>HTML</td><td>-webkit-clip-path</td><td>-webkit-clip-path</td><td>No</td><td>No</td><td></td></tr>

<tr><td>SVG</td><td>-webkit-clip-path</td><td>-webkit-clip-path</td><td>No</td><td>No</td><td></td></tr>

<tr><td rowspan="2"><a href="http://docs.webplatform.org/wiki/css/properties/clip-path">clip-path</a> with SVG path</td><td>HTML</td><td>-webkit-clip-path</td><td>-webkit-clip-path</td><td>No</td><td>No</td><td></td></tr>

<tr><td>SVG</td><td>clip-path</td><td>clip-path</td><td>clip-path</td><td>clip-path</td><td></td></tr>

<tr><td rowspan="2"><a href="http://docs.webplatform.org/wiki/css/properties/mask-image">mask-image</a></td><td>HTML</td><td>-webkit-mask-image</td><td>-webkit-mask-image</td><td>No</td><td>No</td><td>Uses alpha masking by default</td></tr>
<tr><td>SVG</td><td>No</td><td>No</td><td>No</td><td>No</td><td></td></tr>

<tr><td rowspan="2"><a href="http://docs.webplatform.org/wiki/css/properties/mask-border">mask-border-image</a></td><td>HTML</td><td>-webkit-mask-box-image</td><td>-webkit-mask-box-image</td><td>No</td><td>No</td><td></td></tr>
<tr><td>SVG</td><td>No</td><td>No</td><td>No</td><td>No</td><td></td></tr>

<tr><td rowspan="2"><a href="http://docs.webplatform.org/wiki/css/properties/mask">mask</a></td><td>HTML</td><td>No</td><td>No</td><td>mask</td><td>No</td><td></td></tr>
<tr><td>SVG</td><td>mask</td><td>mask</td><td>mask</td><td>mask</td><td>Uses luminance masking by default</td></tr>

<tr><td rowspan="2"><a href="http://docs.webplatform.org/wiki/css/properties/filter">SVG Filter</a></td><td>HTML</td><td>-webkit-filter</td><td>-webkit-filter</td><td>filter</td><td>No</td><td></td></tr>
<tr><td>SVG</td><td>filter</td><td>filter</td><td>filter</td><td>filter</td><td></td></tr>

<tr>
<td><a href="http://html.adobe.com/webplatform/layout/regions/">regions</a></td>
<td>HTML</td>
<td>-webkit-flow-into / -webit-flow-from</td>
<td>No</td>
<td>No</td>
<td>No</td>
<td>Chrome dropped support for regions</td>
</tr>

</tbody>
</table>
