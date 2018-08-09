# Table

## Overview

Tables should only be used to present raw data sets, to make content easy to scan and compare. If used for non-tabular data, this will not adhere to accessibility guidelines. A good example of using a table is to display fee data. Tables outside of rich text editors are responsive, and at smaller screen sizes, the columns and rows stack, turning into a list. Rich text tables have overflow turned on and will scroll on smaller screens.

![](../../.gitbook/assets/table%20%282%29.png)

### Accessibility & Best Practices

## Code

### Table

{% tabs %}
{% tab title="HTML" %}
```markup
<table class="ma__table ">
  <thead>
    <tr>
      <th scope="col">Type</th>
      <th scope="col">Name</th>
      <th scope="col">Fee</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th data-label="Type" scope="row" rowspan="4">Freshwater Fishing</th>
      <td data-label="Name">Resident Citizen or Non-Resident Fishing</td>
      <td data-label="Fee">$27.50</td>
    </tr>
    <tr class="is-offset">
      <td data-label="Name">Resident Citizen or Non-Resident Minor Fishing (Age 15-17)</td>
      <td data-label="Fee">FREE</td>
    </tr>
    <tr class="is-offset">
      <td data-label="Name">Resident Citizen Fishing (Age 65-69)</td>
      <td data-label="Fee">$16.25</td>
    </tr>
    <tr class="is-offset">
      <td data-label="Name">Resident Citizen Fishing (Aged 70 or Over)</td>
      <td data-label="Fee">FREE</td>
    </tr>
  </tbody>
  <tbody>
    <tr>
      <th data-label="Type" scope="row" rowspan="4">Hunting</th>
      <td data-label="Name">Resident Citizen Hunting</td>
      <td data-label="Fee">$27.50</td>
    </tr>
    <tr class="is-offset">
      <td data-label="Name">Resident Citizen Hunting, (Age 65-69)</td>
      <td data-label="Fee">$16.25</td>
    </tr>
    <tr class="is-offset">
      <td data-label="Name">Resident and Non-Resident Citizen Hunting</td>
      <td data-label="Fee">FREE</td>
    </tr>
    <tr class="is-offset">
      <td data-label="Name">Resident Hunting</td>
      <td data-label="Fee">$27.50</td>
    </tr>
  </tbody>
</table>
```
{% endtab %}

{% tab title="React" %}
[Table in Storybook](https://mayflower-react.digital.mass.gov/?knob-href=%23&knob-info=&knob-ButtonSearch.text=Search&knob-HeaderSearch.defaultText=&knob-HeaderSearch.withOrgDropdown=true&knob-ButtonSearch.ariaLabel=Search&knob-tableOptions.feeTable={"head"%3A{"rows"%3A[{"rowSpanOffset"%3Afalse%2C"cells"%3A[{"heading"%3Afalse%2C"colspan"%3A""%2C"rowspan"%3A""%2C"text"%3A"Type"}%2C{"heading"%3Atrue%2C"colspan"%3A""%2C"rowspan"%3A""%2C"text"%3A"Name"}%2C{"heading"%3Atrue%2C"colspan"%3A""%2C"rowspan"%3A""%2C"text"%3A"Fee"}]}]}%2C"bodies"%3A[{"rows"%3A[{"rowSpanOffset"%3Afalse%2C"cells"%3A[{"heading"%3Atrue%2C"colspan"%3A""%2C"rowspan"%3A"4"%2C"text"%3A"Freshwater%20Fishing"}%2C{"heading"%3Afalse%2C"colspan"%3A""%2C"rowspan"%3A""%2C"text"%3A"Resident%20Citizen%20or%20Non-Resident%20Fishing"}%2C{"heading"%3Afalse%2C"colspan"%3A""%2C"rowspan"%3A""%2C"text"%3A"%2427.50"}]}%2C{"rowSpanOffset"%3Atrue%2C"cells"%3A[{"heading"%3Afalse%2C"colspan"%3A""%2C"rowspan"%3A""%2C"text"%3A"Resident%20Citizen%20or%20Non-Resident%20Minor%20Fishing%20%28Age%2015-17%29"}%2C{"heading"%3Afalse%2C"colspan"%3A""%2C"rowspan"%3A""%2C"text"%3A"FREE"}]}%2C{"rowSpanOffset"%3Atrue%2C"cells"%3A[{"heading"%3Afalse%2C"colspan"%3A""%2C"rowspan"%3A""%2C"text"%3A"Resident%20Citizen%20Fishing%20%28Age%2065-69%29"}%2C{"heading"%3Afalse%2C"colspan"%3A""%2C"rowspan"%3A""%2C"text"%3A"%2416.25"}]}%2C{"rowSpanOffset"%3Atrue%2C"cells"%3A[{"heading"%3Afalse%2C"colspan"%3A""%2C"rowspan"%3A""%2C"text"%3A"Resident%20Citizen%20Fishing%20%28Aged%2070%20or%20Over%29"}%2C{"heading"%3Afalse%2C"colspan"%3A""%2C"rowspan"%3A""%2C"text"%3A"FREE"}]}]}%2C{"rows"%3A[{"rowSpanOffset"%3Afalse%2C"cells"%3A[{"heading"%3Atrue%2C"colspan"%3A""%2C"rowspan"%3A"4"%2C"text"%3A"Hunting"}%2C{"heading"%3Afalse%2C"colspan"%3A""%2C"rowspan"%3A""%2C"text"%3A"Resident%20Citizen%20Hunting"}%2C{"heading"%3Afalse%2C"colspan"%3A""%2C"rowspan"%3A""%2C"text"%3A"%2427.50"}]}%2C{"rowSpanOffset"%3Atrue%2C"cells"%3A[{"heading"%3Afalse%2C"colspan"%3A""%2C"rowspan"%3A""%2C"text"%3A"Resident%20Citizen%20Hunting%2C%20%28Age%2065-69%29"}%2C{"heading"%3Afalse%2C"colspan"%3A""%2C"rowspan"%3A""%2C"text"%3A"%2416.25"}]}%2C{"rowSpanOffset"%3Atrue%2C"cells"%3A[{"heading"%3Afalse%2C"colspan"%3A""%2C"rowspan"%3A""%2C"text"%3A"Resident%20and%20Non-Resident%20Citizen%20Hunting"}%2C{"heading"%3Afalse%2C"colspan"%3A""%2C"rowspan"%3A""%2C"text"%3A"FREE"}]}%2C{"rowSpanOffset"%3Atrue%2C"cells"%3A[{"heading"%3Afalse%2C"colspan"%3A""%2C"rowspan"%3A""%2C"text"%3A"Resident%20Hunting"}%2C{"heading"%3Afalse%2C"colspan"%3A""%2C"rowspan"%3A""%2C"text"%3A"%2427.50"}]}]}]}&knob-button.href=https%3A%2F%2Fmass.gov&knob-HeaderSearch.placeholder=Search%20Mass.gov&knob-button.text=button&knob-button.info=this%20will%20be%20the%20tooltip%20text%20on%20hover&knob-ButtonWithIcon.text=BUTTON&knob-HeaderSearch.buttonSearch.ariaLabel=Search&knob-HeaderSearch.orgDropdown.inputText={"boxed"%3Atrue%2C"label"%3Anull%2C"placeholder"%3A"Search%20an%20organization..."%2C"id"%3A"org-typeahead"%2C"options"%3A[{"text"%3A""%2C"value"%3A""}%2C{"text"%3A"Org%20Having%20%28Parentheses%20in%20the%20Name%29"%2C"value"%3A"org-having-parentheses-in-the-name"}%2C{"text"%3A"Attorney%20General's%20Office"%2C"value"%3A"attorney-general-office"}%2C{"text"%3A"Governor's%20Office"%2C"value"%3A"governors-office"}%2C{"text"%3A"Bureau%20of%20Environmental%20Health"%2C"value"%3A"bureau-of-environmental-health"}%2C{"text"%3A"Department%20of%20Conservation%20%26%20Recreation"%2C"value"%3A"department-of-conservation--recreation"}%2C{"text"%3A"Department%20of%20Unemployment%20Assistance"%2C"value"%3A"department-of-unemployment-assistance"}%2C{"text"%3A"495%2FMetroWest%20Suburban%20Edge%20Community%20Commission"%2C"value"%3A"495metrowest-suburban-edge-community-commission"}%2C{"text"%3A"Administrative%20Council%20on%20Toxics%20Use%20Reduction"%2C"value"%3A"administrative-council-on-toxics-use-reduction"}%2C{"text"%3A"Advisory%20Committee%20to%20the%20Administrative%20Council%20on%20Toxics%20Use%20Reduction"%2C"value"%3A"advisory-committee-to-the-administrative-council-on-toxics-use-reduction"}%2C{"text"%3A"Alcoholic%20Beverages%20Control%20Commission"%2C"value"%3A"alcoholic-beverages-control-commission"}%2C{"text"%3A"Appeals%20Court"%2C"value"%3A"appeals-court"}%2C{"text"%3A"Architectural%20Access%20Board"%2C"value"%3A"architectural-access-board"}%2C{"text"%3A"Berkshire%20District%20Attorney%20Paul%20J.%20Caccaviello"%2C"value"%3A"berkshire-district-attorney-paul-j-caccaviello"}%2C{"text"%3A"Board%20of%20Registration%20in%20Dentistry"%2C"value"%3A"board-of-registration-in-dentistry"}%2C{"text"%3A"Board%20of%20Registration%20in%20Medicine"%2C"value"%3A"board-of-registration-in-medicine"}]%2C"selected"%3A""}&knob-button.outline=true&knob-HeaderSearch.orgDropdown.dropdownButton={"text"%3A"All%20Organizations"%2C"capitalized"%3Atrue}&knob-linkText=Lorem%20ipsum%20dolor%20sit%20amet&knob-HeaderSearch.buttonSearch.text=Search&knob-ButtonWithIcon.icon=chevron&selectedKind=atoms%2Ftable&selectedStory=Table&full=0&addons=1&stories=1&panelRight=0&addonPanel=storybooks%2Fstorybook-addon-knobs)
{% endtab %}

{% tab title="Twig PL" %}
[Table in Pattern Lab](https://mayflower.digital.mass.gov/?p=atoms-table)
{% endtab %}
{% endtabs %}

## Style

### Classnames

| **Name** | **scss Modifier** |
| :--- | :--- |
| Table | .ma\_\_table |
| Table Row | .is-offset |
