---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 758d38b9464102ebdfbc425c272494c87398a498
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/19/2019
ms.locfileid: "36462649"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/{id}/attachments')
    .version('beta')
    .get();

```