---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 310bbd17a1a2fb420ee7e2b0cfbb30bb7a7f5d97
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714178"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/{id}/dismissReminder')
    .version('beta')
    .post();

```