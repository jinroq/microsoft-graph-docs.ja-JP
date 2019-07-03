---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b07088575fcb2e086e82c7234a1d87e90a3af73a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35496313"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const Stream = [
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url-or-part-name" alt="image-alt-text" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>new-page-content</li>'
  }
];

let res = await client.api('/me/onenote/pages/{id}/content')
    .update({Stream : Stream});

```