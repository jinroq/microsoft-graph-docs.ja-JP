---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5e07391c2685df21068eb06a248d99558a4e5045
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/11/2019
ms.locfileid: "36838969"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/root/workbook/comments/{id}')
    .version('beta')
    .get();

```