---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a9d575911b7cfa289b301d4d98c0fe74ec3ba326
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715022"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{user-id}')
    .delete();

```