---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9913ccc7e88d13e20968811d14e153707acb7917
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723450"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/owners/{id}/$ref')
    .delete();

```