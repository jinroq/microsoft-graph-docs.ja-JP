---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 00439aa5b96ac7e9cbf9bf744d43573d2d1ed08d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877707"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id}/outlook/tasks/{id}/attachments')
    .version('beta')
    .get();

```