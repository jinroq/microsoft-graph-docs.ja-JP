---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1f67bcd6431d799d6965aab23e138e1b09792ce1
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718707"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/organization/{id}/certificateBasedAuthConfiguration')
    .version('beta')
    .get();

```