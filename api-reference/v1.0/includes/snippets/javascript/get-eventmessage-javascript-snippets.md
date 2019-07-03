---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7f643262fae0c9435c5a485697328772d763fe97
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35472048"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkADYAAAImV_lAAA=')
    .get();

```