---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9d458b6e1a5fbc06c487dab0e385c45808cb8087
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/11/2019
ms.locfileid: "36838718"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/root/workbook/comments/{id}/replies/{id}')
    .version('beta')
    .get();

```