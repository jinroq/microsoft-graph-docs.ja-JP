---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b1e2d9655e2fb2808d176a9a6109c303214a71f0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728293"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/programControls')
    .version('beta')
    .get();

```