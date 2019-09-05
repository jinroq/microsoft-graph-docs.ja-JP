---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fe26c2a1df0a358eb89634097734290b152fdb46
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720116"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/organization/{id}/certificateBasedAuthConfiguration/{id}')
    .version('beta')
    .get();

```