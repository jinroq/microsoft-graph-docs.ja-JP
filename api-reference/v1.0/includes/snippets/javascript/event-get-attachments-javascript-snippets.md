---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7fa1b9317c0a8cda7df79e540a345359e3df4a66
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/19/2019
ms.locfileid: "36462287"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/{id}/attachments')
    .get();

```