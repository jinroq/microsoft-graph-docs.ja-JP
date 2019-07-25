---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6abbf8d8627ec46add62c89547fd4d7dbfaf3f8d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729939"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/lists')
    .version('beta')
    .get();

```