---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2d1920047e3c36c8f6a2110446cd6bdbd604cc47
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731914"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/sectionGroups/{id}')
    .get();

```