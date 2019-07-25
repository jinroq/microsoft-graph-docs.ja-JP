---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9345fd73eb0d2f8a89876986544c4db22b5eae3c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714434"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/synchronizationProfiles/{id}/errors')
    .version('beta')
    .get();

```