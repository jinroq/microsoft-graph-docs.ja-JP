---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a108f67c9b0e4efff113397c5f6ada797be71b7c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711772"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/removeFavorite')
    .version('beta')
    .post();

```