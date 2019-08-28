---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 48c989f3dce93cd1f5c7292434dca56c4e1057f2
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/19/2019
ms.locfileid: "36465004"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/delta(token='1230919asd190410jlka')')
    .version('beta')
    .get();

```