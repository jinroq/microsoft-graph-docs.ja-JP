---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: bce7f3bfb34d02cd2c2d087544f8e38abf260774
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731849"
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
    .post({onenoteSection : onenoteSection});

```