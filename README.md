# पारदर्शी टिप्पणी पुस्तक

इस पुरालेख (repository)  का स्तुति परिचय `ssh` और `https` में।

```
git@github.com:boseji/DocSiteTemplate.git
```

```
https://github.com/boseji/DocSiteTemplate.git
```

## कार्यविधि

यह पुरालेख एक अन्य पुरालेख के आधार पर कार्यविधि को सम्पूर्ण करता हैं |
उस अन्य पुरालेख का स्तुति परिचय यह हैं | 

```
https://github.com/boseji/DocsTemplate
```

अंदरुनी रूप से यह पुरालेख *गिटहब अक्षांस ( Github Actions )* का प्रयोग करता हैं |
इसी कारण वश आपको इन *Actions* का प्रयोग करना होगा | 
आपको पहले *समायोजन व (Settings)* में जा कर कुछ चीजों को सक्षम करना होगा |

- **Actions** में जाकर उसके नीचे **General** उप विषय का चयन करे - 

	- *Artifact and log retention* विषय के नीचे जाकर -
	- **Artifact and log retention** को `1 days` करना होगा |
	- *Workflow permisions* विषय के नीचे जाकर -
	- *Read repository contents and packages permissions* का चयन करना होगा |

- **Pages** में जाकर -
	
	- *Build and deployment* विषय के नीचे जाकर -
	- **Source** को `Deploy from a branch` करना होगा |
	- **Branch** को `gh-pages` नियुक्त करना होगा |
		यह ध्यान में रहे की इस चीजों दोबारा करने की अवश्क्ता पड़ सक्ति है |

इन संयोजनों को समाप्त करने के पश्चात आप २ प्रकार से इस पुरालेख को कार्यरत कर सकते हैं | 

- पुरालेख  के **Action** विषय में जाकर - *Workflows*  विषय के नीच `ci` को कार्यरत करे (Run workflow) |
- इस पुरालेख में *पुनरीक्षण व (Commit)* करके भी चलाया जा सकता हैं |

अंदरुनी या उपयोगित पुरालेख को हमें `ci.yml` में अवश्य बदलना पड़ता हैं | 

```yaml
...
          repository: "boseji/DocsTemplate"
...
```
इस में `boseji/DocsTemplate` को बदल कर आपका `<यूजरनाम>/<पुरालेख>` के रूप में लिखे | 

## अनुज्ञापत्र अथवा `लाइसेंस` (License)

```
(C) Copyright (C) 2024 boseji - All Rights Reserved
This work is licensed under the Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License.
To view a copy of this license, visit http://creativecommons.org/licenses/by-nc-nd/4.0/ or
send a letter to Creative Commons, PO Box 1866, Mountain View, CA 94042, USA.
```

All software, documents, artifacts, files of any type and articles
found in this repository are governed by the following license -

**Attribution-NonCommercial-NoDerivatives 4.0 International (CC BY-NC-ND 4.0)**

<https://creativecommons.org/licenses/by-nc-nd/4.0/>

[LICENSE.txt file](./LICENSE.txt)

`SPDX: CC-BY-NC-ND-4.0`

Contents have been shared under the following terms specified by the above license:

- **Attribution** — You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.

- **NonCommercial** — You may not use the material for commercial purposes.

- **NoDerivatives** — If you remix, transform, or build upon the material, you may not distribute the modified material.

- **No additional restrictions** — You may not apply legal terms or technological measures that legally restrict others from doing anything the license permits.

