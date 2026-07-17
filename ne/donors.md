---
layout: page
lang: ne
nav: donors
title: दाताहरू
lede: मन्दिर निर्माण, जीर्णोद्धार र सेवामा सहयोग गर्ने दाताहरूको सम्मान सूची।
permalink: /ne/donors/
---

{% assign t = site.data.strings.ne %}

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
        <td>{{ donor.name_ne }}</td>
        <td>
          {{ donor.gift_ne }}
          <span class="donor-gift-type">{% if donor.type == 'cash' %}नगद{% else %}वस्तु{% endif %}</span>
        </td>
      </tr>
      {% endfor %}
    </tbody>
  </table>
</div>
