---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ca5cd047ed90488ecf28ddb7189a2835411ff97f
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637830"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const updateMetadata = {
  metadata: "metadata-value",
  clientContext: "clientContext-value"
};

let res = await client.api('/app/calls/{id}/updateMetadata')
    .version('beta')
    .post(updateMetadata);

```