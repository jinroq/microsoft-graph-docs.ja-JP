---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f1e8864c7df9977afb77d2e22dcc9a88eb755684
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709247"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendar')
    .version('beta')
    .delete();

```