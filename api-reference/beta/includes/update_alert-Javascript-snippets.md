---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7d364c6bbca882d937960af1d53b3d519a85c8bd
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465658"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const alert = {
  assignedTo: "String",
  closedDateTime: "String (timestamp)",
  comments: ["String"],
  feedback: "@odata.type: microsoft.graph.alertFeedback",
  status: "@odata.type: microsoft.graph.alertStatus",
  tags: ["String"],
  vendorInformation:
    {
      provider: "String",
      vendor: "String"
    }
};

let res = await client.api('/security/alerts/{alert_id}')
    .version('beta')
    .update({alert : alert});

```