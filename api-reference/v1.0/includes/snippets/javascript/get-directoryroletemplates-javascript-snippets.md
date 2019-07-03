---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8cc2a36df4923164a03f1aee68235c33e6aea331
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35513204"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoleTemplates')
    .get();

```