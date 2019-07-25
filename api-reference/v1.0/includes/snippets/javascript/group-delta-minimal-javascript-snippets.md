---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ef3038091c30f73f7063b8656faf65d8bda3a167
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890872"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/delta')
    .header('Prefer','return=minimal')
    .select('displayName,description,mailNickname')
    .get();

```