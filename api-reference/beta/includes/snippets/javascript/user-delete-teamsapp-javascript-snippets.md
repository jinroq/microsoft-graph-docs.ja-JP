---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 11fd8e9e37156789dcc8ce3bf16164b8499bc09b
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931651"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id}/teamwork/installedApps/{id}')
    .version('beta')
    .delete();

```