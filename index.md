Initial commit

---

Test

{% include_relative src/modules/MMM-AirQuality/MMM-AirQuality.md %}

---

Test 2

{% capture my_include %}{% include src/modules/MMM-AirQuality/MMM-AirQuality.md %}{% endcapture %}
{{ my_include | markdownify }}
