---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6d864e777c0f1bcb3e0a99f0d4ba9124f6552e3f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35496037"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/acceptedSenders')
    .get();

```