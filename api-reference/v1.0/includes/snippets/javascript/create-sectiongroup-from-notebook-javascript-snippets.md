---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1469b5cdfd19975e0c9c9de313fb0f1428c0d60d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730083"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sectionGroup = {
  displayName: "Section group name"
};

let res = await client.api('/me/onenote/notebooks/{id}/sectionGroups')
    .post({sectionGroup : sectionGroup});

```