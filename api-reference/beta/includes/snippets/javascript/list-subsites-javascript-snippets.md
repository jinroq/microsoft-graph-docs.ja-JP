---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6c03eb6eed82af5d6f44020a364f3ae1650d9f9f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717556"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/sites')
    .version('beta')
    .get();

```