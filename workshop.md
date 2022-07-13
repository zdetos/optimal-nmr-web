---
layout: default
title: optimal-nmr Experiments
---
# Workshop Optimal Control in MAS solid-state NMR  {#my-h1-id}

The workshop presents theory and applications of optimal control pulse sequence design in MAS solid-state NMR, 
discusses current developments, and wants to stimulate new ideas for application of optimal control in magnetic resonance.

**Date**: October 13-14, 2022

**Location**:  [Institute of Advanced Studies](https://www.ias.tum.de/ias/institute-for-advanced-study/resources-facilities/ias-building/) of the Technical University Munich in Garching, Germany

#### Program (preliminary) {#my-h4-id}

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
  {% for item in site.data.workshop_program_thursday %}
     <tr>
      <td style="text-align: left">{{ item.time }}</td>
      {% if item.title == " "  %}
         <td style="text-align: center"><strong>{{ item.speaker }}</strong></td>
         <td style="text-align: left"> </td>
      {% else %}
         <td style="text-align: center"><em>{{ item.speaker }}</em></td>
         <td style="text-align: left">
            <div style="width: 400px; text-align: justify">
            {{ item.title }} 
            <details style="font-size: 12px; padding: 5px 20px 5px 5px"><summary>Abstract</summary>
            <p>
               {{ item.abstract }}
            </p> 
            </details>
            </div>
         </td>
      {% endif %}
     </tr>
  {% endfor %}
  </tbody>
</table>

**Friday, Oct 14**

<table>
  <thead>
    <tr>
      <th style="text-align: left">Time</th>
      <th style="text-align: center">Speaker</th>
      <th style="text-align: left">Title</th>
    </tr>
  </thead>
  <tbody>
  {% for item in site.data.workshop_program_friday %}
     <tr>
      <td style="text-align: left">{{ item.time }}</td>
      {% if item.title == " "  %}
         <td style="text-align: center"><strong>{{ item.speaker }}</strong></td>
         <td style="text-align: left"> </td>
      {% else %}
         <td style="text-align: center"><em>{{ item.speaker }}</em></td>
         <td style="text-align: left">
            <div style="width: 400px; text-align: justify">
            {{ item.title }} 
            <details style="font-size: 12px; padding: 5px 20px 5px 5px"><summary>Abstract</summary>
            <p>
               {{ item.abstract }}
            </p> 
            </details>
            </div>
         </td>
      {% endif %}
     </tr>
  {% endfor %}
  </tbody>
</table>
