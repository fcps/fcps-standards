## <a name="useOfColor"></a> Use of Color
<a name="top"></a>

## <a name="nominalColors"></a> Nominal Scale Color Mappings
These colors only serve to help distinguish between comparable groups. The colors are repeated throughout the dashboard tool for a few important reasons :

1. This is the only palette we found that satisfies accessibility standards related to individuals with color sight impairments.
2. The values on a nominal scale do not have any natural order.
3. In cases where there are multiple groups being displayed we wanted to help everyone get in the habit of viewing/checking the legends in the graphs for understanding.
4. If the values on a nominal scale are truly comparable, we don't need multiple color palettes since the colors only serve to identify the groups.

This might be a bit different from what you are used to, but our motive is both to make the information more accessible and to provide you with examples of best practices in data visualization.

When multiple **equivalent groups** are displayed:

<table style="width: 100%;">
    <thead></thead>
    <tbody>
        <tr>
            <td style="background-color: #f3c300; height: 16px;">
                <div style="color: #000000;" align="center">Group 1</div>
            </td>
            <td style="background-color: #875692; height: 16px;">
                <div style="color: #ffffff;" align="center">Group 2</div>
            </td>
        </tr>
    </tbody>
</table>
<table style="width: 100%; margin-bottom: 10px;">
    <tbody>
        <tr>
            <td style="background-color: #f38400; height: 16px;">
                <div style="color: #000000;" align="center">Group 3</div>
            </td>
            <td style="background-color: #a1caf1; height: 16px;">
                <div style="color: #000000;" align="center">Group 4</div>
            </td>
            <td style="background-color: #be0032; height: 16px;">
                <div style="color: #ffffff;" align="center">Group 5</div>
            </td>
            <td style="background-color: #c2b280; height: 16px;">
                <div style="color: #000000;" align="center">Group 6</div>
            </td>
            <td style="background-color: #848482; height: 16px;">
                <div style="color: #ffffff;" align="center">Group 7</div>
            </td>
        </tr>
    </tbody>
</table>

In the rare occassion that there are more than 7 distinct groups:

<table style="width: 100%;">
    <thead></thead>
    <tbody>
        <tr>
            <td style="background-color: #f3c300; height: 16px;">
                <div style="color: #000000;" align="center">Group 1</div>
            </td>
            <td style="background-color: #875692; height: 16px;">
                <div style="color: #ffffff;" align="center">Group 2</div>
            </td>
            <td style="background-color: #f38400; height: 16px;">
                <div style="color: #000000;" align="center">Group 3</div>
            </td>
            <td style="background-color: #a1caf1; height: 16px;">
                <div style="color: #000000;" align="center">Group 4</div>
            </td>
            <td style="background-color: #be0032; height: 16px;">
                <div style="color: #ffffff;" align="center">Group 5</div>
            </td>
        </tr>
        <tr>
            <td style="background-color: #c2b280; height: 16px;">
                <div style="color: #000000;" align="center">Group 6</div>
            </td>
            <td style="background-color: #848482; height: 16px;">
                <div style="color: #ffffff;" align="center">Group 7</div>
            </td>
            <td style="background-color: #008856; height: 16px;">
                <div style="color: #ffffff;" align="center">Group 8</div>
            </td>
            <td style="background-color: #e68fac; height: 16px;">
                <div style="color: #000000;" align="center">Group 9</div>
            </td>
            <td style="background-color: #0067a5; height: 16px;">
                <div style="color: #ffffff;" align="center">Group 10</div>
            </td>
        </tr>
        <tr>
            <td style="background-color: #f99379; height: 16px;">
                <div style="color: #000000;" align="center">Group 11</div>
            </td>
            <td style="background-color: #604e97; height: 16px;">
                <div style="color: #ffffff;" align="center">Group 12</div>
            </td>
            <td style="background-color: #f6a600; height: 16px;">
                <div style="color: #000000;" align="center">Group 13</div>
            </td>
            <td style="background-color: #b3446c; height: 16px;">
                <div style="color: #000000;" align="center">Group 14</div>
            </td>
            <td style="background-color: #dcd300; height: 16px;">
                <div style="color: #000000;" align="center">Group 15</div>
            </td>
        </tr>
        <tr>
            <td style="background-color: #882d17; height: 16px;">
                <div style="color: #ffffff;" align="center">Group 16</div>
            </td>
            <td style="background-color: #8db600; height: 16px;">
                <div style="color: #000000;" align="center">Group 17</div>
            </td>
            <td style="background-color: #654522; height: 16px;">
                <div style="color: #ffffff;" align="center">Group 18</div>
            </td>
            <td style="background-color: #e25822; height: 16px;">
                <div style="color: #ffffff;" align="center">Group 19</div>
            </td>
            <td style="background-color: #2b3d26; height: 16px;">
                <div style="color: #ffffff;" align="center">Group 20</div>
            </td>
        </tr>
    </tbody>
</table>

[Back to the Top](#useOfColor) [Back to Top of Section](#nominalColors) [Back to Table of Contents](#visualizationStandardsTOC)

## <a name="ordinalColors"></a> Ordinal, Intervallic, and Ratio Scale Color Mappings

These color mappings are used when the underlying scale has meaning.  For example, generally when values increase the intensity of the color will also increase.

One exception to this rule of thumb is when we use "divergent" color mappings.  When we want to illustrate the distance from a central point in either direction we'll use divergent color mappings.  For example, on the CogAT assessment - used to identify students for the Gifted/Talented program - higher scores become more green while lower scores become more brown. This visual distinction helps you to quickly identify distance from the mid point.

### <a name="actColors"></a> ACT Score Groups
<table style="width: 100%;">
    <thead></thead>
    <tbody>
        <tr>
            <td style="background-color: #feedde; height: 16px;">
                <div style="color: #000000;" align="center">1-6</div>
            </td>
            <td style="background-color: #fdd0a2; height: 16px;">
                <div style="color: #000000;" align="center">7-12</div>
            </td>
            <td style="background-color: #fdae6b; height: 16px;">
                <div style="color: #ffffff;" align="center">13-18</div>
            </td>
            <td style="background-color: #fd8d3c; height: 16px;">
                <div style="color: #ffffff;" align="center">19-24</div>
            </td>
            <td style="background-color: #e6550d; height: 16px;">
                <div style="color: #ffffff;" align="center">25-30</div>
            </td>
            <td style="background-color: #a63603; height: 16px;">
                <div style="color: #ffffff;" align="center">31-36</div>
            </td>
        </tr>
    </tbody>
</table>

[Back to Top of Section](#ordinalColors) [Back to Table of Contents](#visualizationStandardsTOC)

### <a name="cogatColors"></a> CogAT

#### <a name="cogatAbilityColors"></a> CogAT Ability Levels
<table style="width: 100%;">
    <thead></thead>
    <tbody>
        <tr>
            <td style="background-color: #a6611a; height: 16px; width: 90px;">
                <div style="color: #ffffff;" align="center">Very Low</div>
            </td>
            <td style="background-color: #dfc27d; height: 16px; width: 90px;">
                <div style="color: #000000;" align="center">Below Average</div>
            </td>
            <td style="background-color: #f5f5f5; height: 16px; width: 90px;">
                <div style="color: #000000;" align="center">Average</div>
            </td>
            <td style="background-color: #80cdc1; height: 16px; width: 90px;">
                <div style="color: #000000;" align="center">Above Average</div>
            </td>
            <td style="background-color: #018571; height: 16px; width: 90px;">
                <div style="color: #ffffff;" align="center">Very High</div>
            </td>
        </tr>
    </tbody>
</table>

#### <a name="cogatStanineColors"></a> CogAT Stanines
<table style="width: 100%;">
    <thead></thead>
    <tbody>
        <tr>
            <td style="background-color: #8c510a; height: 16px;">
                <div style="color: #ffffff;" align="center">1</div>
            </td>
            <td style="background-color: #bf812d; height: 16px;">
                <div style="color: #ffffff;" align="center">2</div>
            </td>
            <td style="background-color: #dfc27d; height: 16px;">
                <div style="color: #000000;" align="center">3</div>
            </td>
            <td style="background-color: #f6e8c3; height: 16px;">
                <div style="color: #000000;" align="center">4</div>
            </td>
            <td style="background-color: #f5f5f5; height: 16px;">
                <div style="color: #000000;" align="center">5</div>
            </td>
            <td style="background-color: #c7eae5; height: 16px;">
                <div style="color: #000000;" align="center">6</div>
            </td>
            <td style="background-color: #80cdc1; height: 16px;">
                <div style="color: #000000;" align="center">7</div>
            </td>
            <td style="background-color: #35978f; height: 16px;">
                <div style="color: #ffffff;" align="center">8</div>
            </td>
            <td style="background-color: #01665e; height: 16px;">
                <div style="color: #ffffff;" align="center">9</div>
            </td>
        </tr>
    </tbody>
</table>

[Back to Top of Section](#ordinalColors) [Back to Table of Contents](#visualizationStandardsTOC)

### <a name="kprepColors"></a> KPREP Proficiency Levels
<table style="width: 100%;">
    <thead></thead>
    <tbody>
        <tr>
            <td style="background-color: #f0f9e8; height: 16px;">
                <div style="color: #000000;" align="center">Novice</div>
            </td>
            <td style="background-color: #bae4bc; height: 16px;">
                <div style="color: #000000;" align="center">Apprentice</div>
            </td>
            <td style="background-color: #7bccc4; height: 16px;">
                <div style="color: #000000;" align="center">Proficient</div>
            </td>
            <td style="background-color: #2b8cbe; height: 16px;">
                <div style="color: #ffffff;" align="center">Distinguished</div>
            </td>
        </tr>
    </tbody>
</table>

[Back to Top of Section](#ordinalColors) [Back to Table of Contents](#visualizationStandardsTOC)

### <a name="nweaMapColors"></a> NWEA MAP Quartiles
<table style="width: 100%;">
    <thead></thead>
    <tbody>
        <tr>
            <td style="background-color: #5e3c99; height: 16px; ">
                <div style="color: #ffffff;" align="center">1st - 24th %ile</div>
            </td>
            <td style="background-color: #b2abd2; height: 16px; ">
                <div style="color: #ffffff;" align="center">25th - 49th %ile</div>
            </td>
            <td style="background-color: #fdb863; height: 16px; ">
                <div style="color: #ffffff;" align="center">50th - 74th %ile</div>
            </td>
            <td style="background-color: #e66101; height: 16px; ">
                <div style="color: #ffffff;" align="center">75th - 99th %ile</div>
            </td>
        </tr>
    </tbody>
</table>

[Back to Top of Section](#ordinalColors) [Back to Table of Contents](#visualizationStandardsTOC)

### <a name="psatColors"></a> PSAT %ile Score Groups
<table style="width: 100%;">
    <thead></thead>
    <tbody>
        <tr>
            <td style="background-color: #f1eef6; height: 16px;">
                <div style="color: #000000;" align="center">1st - 20th %ile</div>
            </td>
            <td style="background-color: #d7b5d8; height: 16px;">
                <div style="color: #000000;" align="center">21st - 40th %ile</div>
            </td>
            <td style="background-color: #df65b0; height: 16px;">
                <div style="color: #ffffff;" align="center">41st - 60th %ile</div>
            </td>
            <td style="background-color: #dd1c77; height: 16px;">
                <div style="color: #ffffff;" align="center">61st - 80th %ile</div>
            </td>
            <td style="background-color: #980043; height: 16px;">
                <div style="color: #ffffff;" align="center">81st - 99th %ile</div>
            </td>
        </tr>
    </tbody>
</table>

[Back to Top of Section](#ordinalColors) [Back to Table of Contents](#visualizationStandardsTOC)

### <a name="satColors"></a> SAT %ile Score Groups
<table style="width: 100%;">
    <thead></thead>
    <tbody>
        <tr>
            <td style="background-color: #ffffcc; height: 16px;">
                <div style="color: #000000;" align="center">1st - 20th %ile</div>
            </td>
            <td style="background-color: #a1dab4; height: 16px;">
                <div style="color: #000000;" align="center">21st - 40th %ile</div>
            </td>
            <td style="background-color: #41b6c4; height: 16px;">
                <div style="color: #ffffff;" align="center">41st - 60th %ile</div>
            </td>
            <td style="background-color: #2c7fb8; height: 16px;">
                <div style="color: #ffffff;" align="center">61st - 80th %ile</div>
            </td>
            <td style="background-color: #253494; height: 16px;">
                <div style="color: #ffffff;" align="center">81st - 99th %ile</div>
            </td>
        </tr>
    </tbody>
</table>

[Back to Top of Section](#ordinalColors) [Back to Table of Contents](#visualizationStandardsTOC)

### <a name="widaColors"></a> WIDA ACCESS for EL's Proficiency Levels
<table style="width: 100%;">
    <thead></thead>
    <tbody>
        <tr>
            <td style="background-color: #edf8fb; height: 16px;">
                <div style="color: #000000;" align="center">Entering</div>
            </td>
            <td style="background-color: #ccece6; height: 16px;">
                <div style="color: #000000;" align="center">Emerging</div>
            </td>
            <td style="background-color: #99d8c9; height: 16px;">
                <div style="color: #000000;" align="center">Developing</div>
            </td>
            <td style="background-color: #66c2a4; height: 16px;">
                <div style="color: #ffffff;" align="center">Expanding</div>
            </td>
            <td style="background-color: #2ca25f; height: 16px;">
                <div style="color: #ffffff;" align="center">Bridging</div>
            </td>
            <td style="background-color: #006d2c; height: 16px;">
                <div style="color: #ffffff;" align="center">Reaching</div>
            </td>
        </tr>
        <tr>
            <td style="font-weight: bold; font-size: 18px; color: #ffffff; background: #0033A0; border: 1px solid #FFFFFF;" colspan="6" align="center">WIDA Alt ACCESS</td>
        </tr>
        <tr>
            <td style="background-color: #edf8fb; height: 16px; width: 75px;">
                <div style="color: #000000;" align="center">Initiating</div>
            </td>
            <td style="background-color: #ccece6; height: 16px; width: 75px;">
                <div style="color: #000000;" align="center">Exploring</div>
            </td>
            <td style="background-color: #99d8c9; height: 16px; width: 75px;">
                <div style="color: #000000;" align="center">Engaging</div>
            </td>
            <td style="background-color: #66c2a4; height: 16px; width: 75px;">
                <div style="color: #ffffff;" align="center">Entering</div>
            </td>
            <td style="background-color: #2ca25f; height: 16px; width: 75px;">
                <div style="color: #ffffff;" align="center">Emerging</div>
            </td>
            <td style="background-color: #006d2c; height: 16px; width: 75px;">
                <div style="color: #ffffff;" align="center">Developing</div>
            </td>
        </tr>
    </tbody>
</table>

[Back to the Top](#useOfColor) [Back to Top of Section](#ordinalColors) [Back to Table of Contents](#visualizationStandardsTOC)

## <a name="specialCasesColors"></a> Special Cases

The mapping of course grades might be a bit unexpected at first. Initially, you're likely to think "Hey, why did they list the letter grades in the wrong order?" This is normal and the reason is that you are accustomed to thinking about grades in alphabetical order. But, if the grades were listed in alphabetical order we would run into a different problem - now the values on any axis with grades appear from Greatest to Least instead of Least to Greatest. In other words, the letters in alphabetical order are actually reversing the meaning of our underlying scale.

One of our goals is to provide consistency in the visualizations and consistency in the way in which the visualizations get interpreted. With that in mind, reversing the order of the letter grades makes the letters match the underlying values that are being displayed (e.g., an A is a higher grade than a B so it should appear to the right if it is mapped on the x-axis or the top if it is mapped on the y-axis).

It may make a little bit more sense to see the letter grades represented in a bit more of a mathematical format. Our use of color to map letter grades is illustrating: F < D < C < B < A. So the values increase from left to right. If the letters were in alphabetical order: A > B > C > D > F the letters increase in the opposite direction of the value of the letter grade. In order to prevent everyone from having to decipher whether or not the scale of the axis was reversed, we wanted to map the colors and grades in a way that consistently represented the values of the data.

### <a name="courseGradeColors"></a> Course Grades
<table style="width: 100%; margin-bottom: 10px;">
    <thead></thead>
    <tbody>
        <tr>
            <td style="background-color: #eff3ff; height: 16px; width: 90px;">
                <div style="color: #000000;" align="center">F</div>
            </td>
            <td style="background-color: #bdd7e7; height: 16px; width: 90px;">
                <div style="color: #000000;" align="center">D</div>
            </td>
            <td style="background-color: #6baed6; height: 16px; width: 90px;">
                <div style="color: #000000;" align="center">C</div>
            </td>
            <td style="background-color: #3182bd; height: 16px; width: 90px;">
                <div style="color: #ffffff;" align="center">B</div>
            </td>
            <td style="background-color: #08519c; height: 16px; width: 90px;">
                <div style="color: #ffffff;" align="center">A</div>
            </td>
        </tr>
    </tbody>
</table>

There is something that you will notice when viewing any of the early warning indicator dashboard content. You'll never see a bar or line that shows a value for "No Risk". There are important reasons for having this value in the legend.

1. **All Students** have some degree of risk.
2. The amount of risk exists on a continuum, not a set of four categories.
3. The categories are there to make the amount of risk easier to comprehend<sup>*</sup>

<sup>*</sup><small>For anyone interested, please feel free to <a href="mailto:Drew.Butcher@fayette.kyschools.us?subject=Can%20you%20explain%20why%20continuous%20quantities%20are%20more%20difficult%20to%20comprehend than%20discrete%20categories%20for%20me?">contact the Office of Data, Research, and Accountability</a>.</small>

[Back to the Top](#useOfColor) [Back to Top of Section](#specialCasesColors) [Back to Table of Contents](#visualizationStandardsTOC)

### <a name="ewisColors"></a> Early Warning Indicators

<table style="width: 100%;">
    <tbody>
        <tr>
            <td style="background-color: #fee5d9; height: 16px;">
                <div style="color: #000000;" align="center">No Risk</div>
            </td>
            <td style="background-color: #fcae91; height: 16px;">
                <div style="color: #ffffff;" align="center">Low Risk</div>
            </td>
            <td style="background-color: #fb6a4a; height: 16px;">
                <div style="color: #ffffff;" align="center">Moderate Risk</div>
            </td>
            <td style="background-color: #cb181d; height: 16px;">
                <div style="color: #ffffff;" align="center">High Risk</div>
            </td>
        </tr>
    </tbody>
</table>

[Back to the Top](#useOfColor) [Back to Top of Section](#specialCasesColors) [Back to Table of Contents](#visualizationStandardsTOC)

# References:

<p>Kelly, K. L. (1965). Twenty-two colors of maximum contrast. <em>Color Engineering, 3(26)</em>, pp. 26-27.</p>
<p>Brewer, C. A. (200x). <em>Color Brewer</em>.  Retrieved from: <a href="http://www.ColorBrewer.org" target="_blank">http://www.ColorBrewer.org</a>, Retrieved on: 22mar2018</p>

[Back to the Top](#useOfColor) [Back to Table of Contents](#visualizationStandardsTOC)