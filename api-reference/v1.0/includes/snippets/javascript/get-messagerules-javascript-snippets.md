---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2f8830c001b746892f38d63bea30b3a46ba9e857
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35704932"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/inbox/messageRules')
    .get();

```