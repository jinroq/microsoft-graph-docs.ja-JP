---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b06a973ba7f7e7b3f2254c415ce217a71a47355c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733515"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/domains/contoso.com')
    .get();

```