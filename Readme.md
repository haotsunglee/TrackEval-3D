# TrackEval-3D
Extend the TrackEval to 3D bounding boxes

This work extends https://github.com/JonathonLuiten/TrackEval/blob/master/docs/MOTChallenge-Official/Readme.md, which can only accept 2D detections. 

## Data Format
<p>
The tracker file format should be the same as the ground truth file, 
which is a CSV text-file containing one object instance per line.
Each line must contain these follwoing values:
</p>

</p>
<code>
&lt;frame&gt;,
&lt;id&gt;,
&lt;x1&gt;,
&lt;x2&gt;,
&lt;x3&gt;,
&lt;x4&gt;,
&lt;x5&gt;,
&lt;x6&gt;,
&lt;x7&gt;,
&lt;x8&gt;,
&lt;y1&gt;,
&lt;y2&gt;,
&lt;y3&gt;,
&lt;y4&gt;,
&lt;y5&gt;,
&lt;y6&gt;,
&lt;y7&gt;,
&lt;y8&gt;,
&lt;z1&gt;,
&lt;z2&gt;,
&lt;z3&gt;,
&lt;z4&gt;,
&lt;z5&gt;,
&lt;z6&gt;,
&lt;z7&gt;,
&lt;z8&gt;,
&lt;-1&gt;,
&lt;-1&gt;,
&lt;-1&gt;,
&lt;-1&gt;
</code>
</p>

The coordinates <code>xn,yn,zn</code> are 8 corner points of each 3D bounding box cuboid.

All frame numbers, target IDs are 1-based. 