---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d968d04c0a552b4b3af4e70071b0954ecb7cd158
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731109"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationSchool = {
  displayName: "Fabrikam High School",
  description: "Magnate school for the arts. Los Angeles School District",
  status: "String",
  externalSource: "String",
  principalEmail: "AmyR@fabrikam.com",
  principalName: "Amy Roebuck",
  externalPrincipalId: "14007",
  highestGrade: "12",
  lowestGrade: "9",
  schoolNumber: "10002",
  address: {
    city: "Los Angeles",
    countryOrRegion: "United States",
    postalCode: "98055",
    state: "CA",
    street: "12345 Main St."
  },
  externalId: "10002",
  fax: "+1 (253) 555-0101",
  phone: "+1 (253) 555-0102",
};

let res = await client.api('/education/schools')
    .post({educationSchool : educationSchool});

```