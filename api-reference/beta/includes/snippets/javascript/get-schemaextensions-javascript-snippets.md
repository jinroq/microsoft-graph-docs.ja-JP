---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d2942f25f94042e2dde70e9f3876a5733e27e692
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718066"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/schemaExtensions')
    .version('beta')
    .filter('id eq 'graphlearn_test'')
    .get();

```