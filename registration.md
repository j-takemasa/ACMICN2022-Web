---
layout: default
title: Registration Information

registrations:
  fees:
    - type: Conference Registration (Author, On-site)
      price: ["$400","$450","$450","$500"]
    - type: Conference Registration (Non-author, On-site)
      price: ["$400","$450","$450","$500"]      
    - type: Conference Registration (Non-author, Virtual)
      price: ["$100","$120","$120","$140"]
    - type: Student Registration (Non-author, On-site)
      price: ["$100","$120","$120","$140"]
    - type: Student Registration (Non-author, Virtual)
      price: ["$20","$30","$30","$40"]
---

## Registration Information

<div class="border ui-corner-all ui-shadow">
  <table class="sponsorlevels">
    <tbody>
      <tr>
        <th style="text-align:left"></th>
        <th>ACM Member (By 31 Aug.)</th>
        <th>ACM Member (After 31 Aug.)</th>
        <th>Non-ACM Member (By 31 Aug.)</th>
        <th>Non-ACM Member (After 31 Aug.)</th>
      </tr>
      {% for reg in page.registrations.fees %}
      <tr>
        <th style="text-align:left">{{ reg.type }}</th>
        <td> {{ reg.price[0] }} </td>
        <td> {{ reg.price[1] }} </td>
        <td> {{ reg.price[2] }} </td>
        <td> {{ reg.price[3] }} </td>
      </tr>
      {% endfor %}
    </tbody>
  </table>
</div>

- On-site Conference Registration includes main conference, tutorials, lunch, coffee and dinner. 
- Student Registration includes main conference, tutorials, lunch and coffee. 

[Online registration](https://cvent.me/7Pl3PL){: data-role="button" class="button" }

In case of problems with registration or billing, please contact [Registration Chair](mailto:icn22.registration-chairs@k2.ics.es.osaka-u.ac.jp).


### A Special Note on Author Registration Policy

- Each accepted full-paper/short-paper/poster/demo must be accompanied by an On-site Conference Registration (neither of a Virtual Conference Registration and a Student Registration). Each On-site Conference Registration can cover up to two (2) full-papers/short-papers/posters/demos, in any combination.
- Each accepted paper, poster, and demo must provide a pre-recording and be in-person or virtually presented by one of its author(s) at the conference. The presenting author(s) must be registered for the conference.
- Registration accepts Visa, MasterCard, American Express.
