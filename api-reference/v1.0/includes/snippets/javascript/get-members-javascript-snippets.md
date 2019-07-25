---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 247493fba342f37d38a991bfd5478d5e88b83f69
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715547"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/members')
    .get();

```