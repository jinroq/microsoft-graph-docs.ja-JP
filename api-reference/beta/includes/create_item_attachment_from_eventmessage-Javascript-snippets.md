---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 09deb6b70ff7fc17c45463ee42764a5963928b2f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34453692"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  @odata.type: "#Microsoft.OutlookServices.ItemAttachment",
  name: "name-value",
  item: "message or event entity"
};

let res = await client.api('/me/events/{id}/attachments')
    .post({attachment : attachment});

```