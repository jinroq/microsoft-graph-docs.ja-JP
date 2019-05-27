---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b30d372de18860269bde1849a7a9f3f01d2abb3f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34434463"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const bookingBusiness = {
    displayName:"Fourth Coffee",
    address:{
        type:"mall",
        postOfficeBox:"P.O. Box 123",
        street:"4567 Main Street",
        city:"Buffalo",
        state:"NY",
        countryOrRegion:"USA",
        postalCode:"98052"
    },
    phone:"206-555-0100",
    email:"manager@fourthcoffee.com",
    webSiteUrl:"https://www.fourthcoffee.com",
    defaultCurrencyIso:"USD"
};

let res = await client.api('/bookingBusinesses')
    .version('beta')
    .post({bookingBusiness : bookingBusiness});

```