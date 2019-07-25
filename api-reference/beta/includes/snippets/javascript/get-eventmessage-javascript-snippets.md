---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: efe03e7d495070275d9c085319cf3af5358c6e3b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712383"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkADYAAAImV_lAAA=')
    .version('beta')
    .get();

```