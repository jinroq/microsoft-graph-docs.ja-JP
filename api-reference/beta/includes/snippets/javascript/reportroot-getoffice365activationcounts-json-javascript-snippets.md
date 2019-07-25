---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7147fd71f9a33c55f910e3f446d279f860db06a9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719486"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365ActivationCounts')
    .version('beta')
    .get();

```