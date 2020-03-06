**SpectraSearch Spring Semester Update**

(post-conference)



**Requirements**

**SPD FUNCTIONS**

| NAME | NAME2 | COMMENTS | ~ |
| --- | --- | --- | --- |
| CCT | Correlated Color Temperature | _Legacy_ | F |
| CRI | Color Rendering Index | General + Extended (R1-R15)(Average Color Fidelity, Old)_Legacy_ | F |
| IES TM-30-2015 Fidelity Index (Rf) | CRI, 99 CES | (Average Color Fidelity, New) | 1 |
| Gamut Index (Rg) | TM-30 | Compares the area enclosed by the average chromaticity coordinates in each of 16 hue bins to characterize the average saturation level of the test source compared to the reference illuminant. A neutral score is 100, with values greater than 100 indicating an increase in saturation and values less than 100 indicating a decrease in saturation. The range in values grows as fidelity decreases. | 1 |
| Hue Fidelity IndicesRf,hj (j = 1 to 16) | TM-30 | Provides a numerical characterization of color fidelity in each of 16 hue bins (j), which can be used to evaluate how similarly the test source renders reds, yellows, greens, blues, or in-between hues compared to the reference. Values range from 0 to 100. Specificvalues may be used to supplement average values if one hue type is of particular concern. Specifying limits for all values is also possible. These scores are analogous to the special indices of the CRI system (e.g., R9), but are more robust because they combineseveral samples with different spectral features. | 1 |
| Chroma Change by HueIndicesRcs,hj (j = 1 to 16) | ™-30 | Provides numerical values for relative chroma change in each of 16 hue bins (j), which can be used to evaluate saturation (positive values) or desaturation (negative values) of reds, yellows, greens,blues, and in-between hues compared to the reference. Supplementary criteria could be set for all values, or just specific values,such as red (bin 1). | 3 |
| Skin Fidelity IndexRf,skin | ™-30 | Characterizes the similarity of skin tones (CES15 and CES18) as rendered by the test source compared to the reference source.Values range from 0 to 100. Rf,skin can be used to supplement other values when skin is an important consideration. | 3 |
| Sample Fidelity IndicesRf,CESi(i = 1 to 99) | ™-30 | Characterizes the similarity of each CES (i) as rendered by the test source compared to the reference source. Values range from 0 to 100. Individual values may have little predictive power for other objects, but examining the scores in a combined chart can indicate the source&#39;s object-to-object consistency. | 3 |
| Chromaticity Coordinates |   | CIE X,Y,X_Legacy_ | 2 |
| Melanopic/Photopic ratio | M/P | Melanopic response in humans for alertness/sleep[Several methods for calculating](https://www.ies.org/fires/m-p-ratios-can-we-agree-on-how-to-calculate-them/) | 2 |
| Scotopic/Photopicratio | S/P | Low-light human responseHelps determine light to energy ratio_energy_ | 2 |
| Luminaire Efficacy Rating | LER | how much light does it put out based on how much energy it consumes//pres joy per joule_energy_ | 3 |
| Lumens per Watt | LPW | _energy_ | 3 |
| CIE S 026 action spectra | α-opic | five human α-opic photoreceptor classes (S-cones, M-cones, L-cones, rods and ipRGCs)_Also see M/P_ | 1 |



**GRAPHICS**

| Name | Place | Comments |
| --- | --- | --- |
| SPD Graph | fund. | SpectralData + Extended tables |
| Color Vector Graphic | TM-30 | Provides a visual representation of hue and saturation changes based on the average rendering in each hue bin, relative to the reference. The graphic provides a quick understanding of how different hues are rendered in different ways. |
| Color Saturation Graphic | TM-30 | Provides a simplified visual representation of only saturation changes based on the average performance in each hue bin. |
| ... | ... | ... |



**OTHER**

- Admin page
- Upload data formats
- Download data formats



**Notes**

**NOTED CHANGES**

- Revert to Sprint 2 Database schema (i.e. separate Spectral Data table) OR attempt unstructured (Final pres.)
- SpectralDataExtendedInfra (rec) and SpectralDataExtendedUltra (TBD)
- Option: Upload to Calculate, but not to Integrate
- SpectraSearch not Spectra Search
- Check _Energy_ SPD functions for matching req in database schema (i.e. Watts)

**Upcoming TBD**

- Ed. page (i.e. how to read)
- DOE Meeting Schedule
- [lux](https://fluxometer.com/rainbow/#!id=iPad%20Pro/6500K-iPad%20Pro) contact (Wyatt/Bryan)



**Planning**

**CALENDAR**

| Scrum Date | Agenda | Comments |
| --- | --- | --- |
| 2/21/20 | Planning, _Begin Sprint 1_ |   |
| 2/28/20 | Scrum |   |
| 3/6/20 | _Begin Sprint 2_ |   |
| March TBD | DOE Meeting |   |
| 3/13/20 |   | Spring Break |
| 3/20/20 | _Begin Sprint 3_ |   |
| 3/23/20 | Midterm Presentation (Owrang) |   |
| 3/27/20 | Scrum |   |
| 4/3/20 | Scrum |   |
| April TBD | DOE Meeting |   |
| 4/10/20 | _Begin Sprint 4_ |   |
| 4/17/20 | _Begin Sprint 5_ |   |
| 4/24/20 | Final Project/Report Due (Owrang) |   |
| April TBD | Last DOE Meeting (Pre-Handoff) |   |
| 5/04/20 | Final Presentation (Owrang) |   |
| May TBD | Handoff to DOE / Final Meeting | End of Semester |



**SPRINTS** (Proposed)

Sprint 1:

- Database
  - Confirm Database SpectralData changes (structured vs unstructured, extended)
- Front-end
  - SPD Graphic Integration Multi-Attempt
    - ■■Rebecca (?)
    - ■■Elisabetta (?)
    - ■■Lily (P5)
- Backend
  - Check _Energy_ SPD Functions reqs to database schema
  - Gather SPD Functions pure formulas
    - ■■~Wave1 and ~Wave2
    - ■■Lily / Matt
- DOE Feb. Meeting
- F.lux

Sprint 2:

- Front-end
  - SPD Graphic Integration Leftovers
  - Begin Admin Page and associated
- Backend
  - Implement ~Wave1 and ~Wave2 SPD Functions
  - Gather SPD Functions pure formulas
    - ■■~Wave3, Sprint 1 leftovers (I imagine M/P)
- DOE Meeting (User Testing @frontend?)

Sprint 3:

- Backend
  - Implement ~Wave3 and leftovers
- Frontend
  - Admin Page and associated finish
  - GRAPHICS table
- Mixed
  - Upload/Download
- Database
  - Extend example data (DOE, Lily)

Sprint 4:

- Testing
  - SPD Functions with extended example data
  - Upload/Download
  - User interface (in-house)
- Ed. Page
- DOE Meeting (User testing)

Sprint 5:

- Implementations based on Sprint 4 user testing
- Front-end polish
- Backend leftovers
