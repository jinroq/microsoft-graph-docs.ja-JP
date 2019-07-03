---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6fc26052e0b9848ceb750096bb949f343125d0e1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35503821"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  accountEnabled: true,
  assignedLicenses: [
    {
      disabledPlans: [ "bea13e0c-3828-4daa-a392-28af7ff61a0f" ],
      skuId: "skuId-value"
    }
  ],
  assignedPlans: [
    {
      assignedDateTime: "2016-10-19T10:37:00Z",
      capabilityStatus: "capabilityStatus-value",
      service: "service-value",
      servicePlanId: "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  businessPhones: [
    "businessPhones-value"
  ],
  city: "city-value"
};

let res = await client.api('/me')
    .version('beta')
    .update({user : user});

```