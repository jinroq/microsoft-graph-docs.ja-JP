---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ede3a5c2d8880becb5f35825177ce31c5bb79fd7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713671"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/events')
    .version('beta')
    .get();

```