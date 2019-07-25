---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ce5fe3c4b243505372b911946d00271ffe69ec0a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712773"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/versions/{version-id}/content')
    .version('beta')
    .get();

```