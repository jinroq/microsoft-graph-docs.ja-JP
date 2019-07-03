---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9b3039f508192013f4b74e99c20b5b8a06a1bef1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35495797"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/plans/{id}')
    .delete();

```