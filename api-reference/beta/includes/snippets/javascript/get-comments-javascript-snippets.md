---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a88b1e0cf8179311e0dab4857762090d4d93147e
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/11/2019
ms.locfileid: "36838887"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/root/workbook/comments')
    .version('beta')
    .get();

```