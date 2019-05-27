---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a3f678005ebb6cab695e5573b4636bcc2b9a88ed
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447636"
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