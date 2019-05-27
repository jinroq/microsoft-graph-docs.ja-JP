---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9f9e78613bbd9fc6f630af55acf8cbd1a4d0d070
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34467896"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/groupLifecyclePolicies')
    .version('beta')
    .get();

```