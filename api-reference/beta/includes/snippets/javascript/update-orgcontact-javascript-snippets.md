---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1d58341adad144b0aa9b512cb8caf10b583d0c50
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637929"
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
    .update(orgContact);

```