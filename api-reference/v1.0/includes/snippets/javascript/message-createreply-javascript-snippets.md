---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e5d3e45cae234a9131ce07b20cbb6e4a881f72b4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732201"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/{id}/createReply')
    .post();

```