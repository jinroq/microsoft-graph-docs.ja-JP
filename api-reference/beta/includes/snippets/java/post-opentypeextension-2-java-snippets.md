---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e54ba2d81fea58502cef6138e872ff22823fa1ff
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878414"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Extension extension = new Extension();
extension.additionalDataManager().put("@odata.type", new JsonPrimitive("microsoft.graph.openTypeExtension"));
extension.extensionName = "Com.Contoso.Referral";
extension.companyName = "Wingtip Toys";
extension.dealValue = 500050;
extension.expirationDate = "2015-12-03T10:00:00Z";

graphClient.me().messages("AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===").extensions()
    .buildRequest()
    .post(extension);

```