---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0ef19d9b84f1d6921e31f20364684022ebddabb1
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459914"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sectionGroup = {
  displayName: "Section group name"
};

let res = await client.api('/me/onenote/sectionGroups/{id}/sectionGroups')
    .post({sectionGroup : sectionGroup});

```