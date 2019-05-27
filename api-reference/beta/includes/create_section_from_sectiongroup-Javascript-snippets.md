---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 052e68ff451e47635264acf4bf91cfaea7d08edf
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439576"
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