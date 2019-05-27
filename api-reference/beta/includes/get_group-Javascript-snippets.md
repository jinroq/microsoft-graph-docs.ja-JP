---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2aae756fcaa1b5602eb752703b71591eefb8c2b1
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34471104"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4')
    .version('beta')
    .get();

```