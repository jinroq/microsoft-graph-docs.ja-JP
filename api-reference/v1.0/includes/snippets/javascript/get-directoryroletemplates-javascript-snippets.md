---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8cc2a36df4923164a03f1aee68235c33e6aea331
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733578"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoleTemplates')
    .get();

```