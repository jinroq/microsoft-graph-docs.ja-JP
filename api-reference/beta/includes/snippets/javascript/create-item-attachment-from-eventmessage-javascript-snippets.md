---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7fcee4b00c818bb1b0299eaa670cdfb2de90d2cb
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/19/2019
ms.locfileid: "36464983"
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
    .version('beta')
    .post({attachment : attachment});

```