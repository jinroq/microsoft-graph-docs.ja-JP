---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9fe36f9bcfbc49c4fb72fbb9e6615066449befd0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729541"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/{id}/send')
    .version('beta')
    .post();

```