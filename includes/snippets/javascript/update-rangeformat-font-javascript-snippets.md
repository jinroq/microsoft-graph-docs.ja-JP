---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a6c1ea5c6767446628a291f431c70ae67763f57a
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36638024"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFont = {
  bold: true,
  color: "#4B180E",
  size: 26
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/font')
    .update(workbookRangeFont);

```