---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 052e68ff451e47635264acf4bf91cfaea7d08edf
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717920"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onenoteSection = {
  displayName: "Section name"
};

let res = await client.api('/me/onenote/sectionGroups/{id}/sections')
    .version('beta')
    .post({onenoteSection : onenoteSection});

```