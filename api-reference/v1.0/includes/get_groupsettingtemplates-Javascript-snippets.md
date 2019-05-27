---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8cd991dae06278d77a74bd69fd3de70678eef6dd
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463028"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groupSettingTemplates')
    .get();

```