---
title: applicationServicePrincipal リソースの種類
description: アプリケーションと servicePrincipal の組み合わせ。
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c3a6d0d1017f89587f1f826c4225eefc51dc5edb
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/22/2019
ms.locfileid: "35147928"
---
# <a name="applicationserviceprincipal-resource-type"></a>applicationServicePrincipal リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD アプリケーションギャラリーからアプリケーションのインスタンスが追加されると、 [application](../resources/application.md)および[serviceprincipal](../resources/serviceprincipal.md)オブジェクトがディレクトリに作成されます。 **Applicationserviceprincipal**は、 **Application**と**serviceprincipal**オブジェクトの連結を表します。

## <a name="methods"></a>メソッド

None

## <a name="properties"></a>プロパティ

| プロパティ | 型        | 説明 |
|:-------------|:------------|:------------|
|application|[application](../resources/application.md)|Azure Active Directory に登録されているアプリケーションを表します。|
|servicePrincipal|[servicePrincipal](../resources/serviceprincipal.md)|ディレクトリ内のアプリケーションのインスタンスを表します。|

## <a name="relationships"></a>リレーションシップ

なし

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationServicePrincipal",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
   "servicePrincipal": {"@odata.type":"microsoft.graph.servicePrincipal"},
   "application": {"@odata.type":"microsoft.graph.application"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationServicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
