---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 49c0bea4151147a5d9bc07a4539214184e092f54
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35895562"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contacts')
    .version('beta')
    .select('displayName,emailAddresses')
    .get();

```