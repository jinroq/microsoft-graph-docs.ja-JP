---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: bd2ea7b6fc8bd396b33ca8f2a82ccb0db76c9150
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715659"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/threads/{id}/posts')
    .get();

```