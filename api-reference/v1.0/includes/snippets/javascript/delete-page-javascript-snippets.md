---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7b3c24aa119cec9f63e8cb2c4b902d0e4ec5822a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732878"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/pages/{id}')
    .delete();

```