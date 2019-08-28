---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f523daa090fe99ad546b78ea78e77bd97de1c81c
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461237"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/me/assignments/{id}/rubric')
    .version('beta')
    .get();

```