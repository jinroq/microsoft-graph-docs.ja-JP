---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b7fb9addbfb14c0b3016b2916ac5092b5d21f15f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733599"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoleTemplates/{id}')
    .get();

```