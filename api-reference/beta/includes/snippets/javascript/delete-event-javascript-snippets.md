---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7ab3f924b99200170176403322dd53d13ba8da71
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712297"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/{id}')
    .version('beta')
    .delete();

```