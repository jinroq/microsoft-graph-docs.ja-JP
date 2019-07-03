---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 57e3301e2bbe01fd3b8d8d16b88f714025a97d74
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35472107"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/buckets/{bucket-id}')
    .get();

```