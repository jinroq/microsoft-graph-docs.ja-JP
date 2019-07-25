---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1c8f2ae8d0801ad636c9dd39dbd44be28b0e05b1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723827"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const convertIdResult = {
  "inputIds" : [
    "{rest-formatted-id-1}",
    "{rest-formatted-id-2}"
  ],
  sourceIdType: "restId",
  targetIdType: "restImmutableEntryId"
};

let res = await client.api('/me/translateExchangeIds')
    .version('beta')
    .post(convertIdResult);

```