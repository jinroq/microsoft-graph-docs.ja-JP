---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6d864e777c0f1bcb3e0a99f0d4ba9124f6552e3f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732444"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/acceptedSenders')
    .get();

```