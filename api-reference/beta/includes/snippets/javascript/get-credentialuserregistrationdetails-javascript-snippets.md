---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9fb13a08a670e7ef69804cd28d90deea303ef110
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871206"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/credentialUserRegistrationDetails')
    .version('beta')
    .get();

```