---
title: 'Download all national indicators from chosen goal'
type: 'GET'
name: '/api/v1/en/national/{goal}.json'
lang: 'en'
---

This method allows users to download data and metadata for all national indicators from chosen goal in English.

### Parameters

<table id='api_table'>
  <tr>
    <th><b>Name</b></th>
    <th><b>Description</b></th>
  </tr>
  <tr>
    <td><b>goal</b></td>
    <td>number of indicator's goal ( 1 - 17 )</td>
  </tr>
</table>

<p style='float:left;margin-top: 7px;'>Response content type</p>
<select style='float:left;padding: 0px 15px;width: 155px;margin-left: 10px;text-align-last: center;'>
  <option>application/json</option>
</select>

<div id='exampleKraj1'>

<h3 id="przykładowy-curl">Curl example</h3>

<p><code class="highlighter-rouge">curl -H "Accept:application/vnd.github.v3.raw" "https://api.github.com/repos/statisticspoland/sdg-indicators-pl/contents/api/v1/en/national/1.json"</code></p>

<h3 id="przykładowy-url">URL example</h3>

<p><code class="highlighter-rouge">https://api.github.com/repos/statisticspoland/sdg-indicators-pl/contents/api/v1/en/national/1.json</code></p>

<h3 id="przykładowy-kod-odpowiedzi">Response code</h3>

<p><code class="highlighter-rouge">200</code></p>

<h3 id="przykładowa-odpowiedź">Response</h3>

<p><code class="highlighter-rouge" id="show-data-kraj-1-en">
</code></p>

</div>

<script>

$.getJSON('https://sdg.gov.pl/api/v1/en/national/1.json', function(data) {
    $('#show-data-kraj-1-en').html(JSON.stringify(data, null, 2));
});

</script>
