---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 08fff3ff7878abe74ec5f504af809a60575a3031
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722886"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups')
    .get();

```