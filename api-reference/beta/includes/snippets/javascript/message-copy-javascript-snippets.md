---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: bed22468e6ad7a2d56814394b65c1a01a135aa5d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721538"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  destinationId: "destinationId-value"
};

let res = await client.api('/me/messages/{id}/copy')
    .version('beta')
    .post(message);

```