---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 67c10e9f52ad598fc92d0584dd5a6f1273a4eabd
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714742"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/conversations/{id}')
    .get();

```