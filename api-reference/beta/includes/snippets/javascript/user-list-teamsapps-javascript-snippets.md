---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5f10204fc4151cf599297f43cbfa6e6f858bf66e
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931337"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id}/teamwork/installedApps')
    .version('beta')
    .get();

```