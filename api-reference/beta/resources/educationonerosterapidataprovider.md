---
title: educationOneRosterApiDataProvider リソース
description: OneRoster API が入力ソースとして使用されている場合に、学校データ同期プロファイルを設定するために使用されます。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ca94043fdf215d47a1ccaf16f3a667f1178c1d57
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972636"
---
# <a name="educationonerosterapidataprovider-resource"></a>educationOneRosterApiDataProvider リソース

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[ONEROSTER API](https://www.imsglobal.org/activity/onerosterlis)が入力ソースとして使用されている場合に、学校データ同期プロファイルを設定するために使用されます。

[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)から派生します。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **connectionUrl** | String | OneRoster インスタンスへの接続 URL。 |
| **schoolsIds** | 文字列コレクション |  同期する school sourcedIds のリスト。 |
| **プロバイダー** | String | [OneRoster 仕様](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA)で定義されている OneRoster サービスプロバイダー名。 |
| **connectionSettings** | [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md) | OneRoster インスタンスの接続設定。 [EducationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md)または[educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md)の種類である必要があります。 |
| **ユーザー** | [educationSynchronizationCustomizations](educationsynchronizationcustomizations.md) | 同期プロファイルに適用されるカスタマイズ (オプション)。|

## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider",
    "connectionUrl": "String",
    "providerName": "String",
    "schoolsIds": [
        "String"
    ],
    "connectionSettings": {
        "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
        "clientId": "String",
        "clientSecret": "String",
    },
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
