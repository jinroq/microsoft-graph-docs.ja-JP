---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a3f678005ebb6cab695e5573b4636bcc2b9a88ed
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730345"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/tasks/'id'/progressTaskBoardFormat')
    .version('beta')
    .get();

```