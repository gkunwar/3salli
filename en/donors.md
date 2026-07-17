---
layout: page
lang: en
nav: donors
title: Donors
lede: Honouring those who support temple construction, care, and service.
permalink: /en/donors/
---

{% assign t = site.data.strings.en %}

<p class="donor-note">{{ t.donors_note }}</p>

<div class="donor-table-wrap">
  <table class="donor-table">
    <thead>
      <tr>
        <th>{{ t.donors_name }}</th>
        <th>{{ t.donors_gift }}</th>
      </tr>
    </thead>
    <tbody>
      {% for donor in site.data.donors %}
      <tr>
        <td>{{ donor.name_en }}</td>
        <td>
          {{ donor.gift_en }}
          <span class="donor-gift-type">{% if donor.type == 'cash' %}Cash{% else %}Material{% endif %}</span>
        </td>
      </tr>
      {% endfor %}
    </tbody>
  </table>
</div>
