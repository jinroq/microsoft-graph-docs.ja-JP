---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: af591176597740220c211b93ad098551bc6d7a5e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728718"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/app/calls/{id}/participants/{id}')
    .version('beta')
    .get();

```