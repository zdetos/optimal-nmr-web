---
layout: default
title: optimal-nmr Experiments
---
# Workshop Optimal Control in MAS solid-state NMR  {#my-h1-id}

**Date**: October 13-14, 2022

**Location**:  [Institute of Advanced Studies](https://www.ias.tum.de/ias/institute-for-advanced-study/resources-facilities/ias-building/) of the Technical University Munich in Garching, Germany

#### Program  {#my-h4-id}

**Thursday, Oct 13**

<table>
  <thead>
    <tr>
      <th style="text-align: left">Time</th>
      <th style="text-align: center">Speaker</th>
      <th style="text-align: left">Title</th>
    </tr>
  </thead>
  <tbody>
  {% for item in site.data.workshop_program_test %}
     <tr>
      <td style="text-align: left">{{ item.time }}</td>
      <td style="text-align: center"><em>{{ item.speaker }}</em></td>
      <td style="text-align: left">{{ item.title }}<br /> 
         <details><summary>Abstract</summary>
         <p style="font-size: 12px; width: 300px; text-align: justify">
         {{ item.abstract }}
         </p> 
         </details>
      </td>
     </tr>
  {% endfor %}
  </tbody>
</table>

