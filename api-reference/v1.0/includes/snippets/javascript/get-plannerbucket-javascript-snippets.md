---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 57e3301e2bbe01fd3b8d8d16b88f714025a97d74
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740606"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/buckets/{bucket-id}')
    .get();

```