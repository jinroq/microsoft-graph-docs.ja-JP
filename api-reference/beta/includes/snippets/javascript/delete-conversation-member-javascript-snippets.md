---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ac5671ce4013f15e03ef113c5a063ea40ae03a3a
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36634010"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/channels/{id}/members/{id}')
    .version('beta')
    .delete();

```