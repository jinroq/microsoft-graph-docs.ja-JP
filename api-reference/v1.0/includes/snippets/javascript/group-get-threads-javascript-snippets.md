---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9e844a9d15987e49ba55b73ade54f7b6b00f6f6c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888182"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/threads')
    .get();

```