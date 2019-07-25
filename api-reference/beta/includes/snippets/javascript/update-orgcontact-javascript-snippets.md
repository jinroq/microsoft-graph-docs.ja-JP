---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 066ebd0e00f5f6b1f7f5a117ae24fe4b765c6693
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729023"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const orgContact = {
  businessPhones: [
    "businessPhones-value"
  ],
  city: "city-value",
  companyName: "companyName-value",
  country: "country-value",
  department: "department-value",
  displayName: "displayName-value"
};

let res = await client.api('/contacts/{id}')
    .version('beta')
    .update({orgContact : orgContact});

```