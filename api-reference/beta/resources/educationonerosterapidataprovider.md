---
title: educationOneRosterApiDataProvider リソース
description: OneRoster API は、入力ソースとして使用するときに、学校のデータの同期プロファイルを設定するために使用します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 681a3331aba7bc84ac80911c4be8076d104f8a58
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938147"
---
# <a name="educationonerosterapidataprovider-resource"></a>educationOneRosterApiDataProvider リソース

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[OneRoster API](https://www.imsglobal.org/activity/onerosterlis)は、入力ソースとして使用するときに、学校のデータの同期プロファイルを設定するために使用します。

[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)から派生します。

## <a name="properties"></a>プロパティ

| プロパティ | 種類 | 説明 |
|:-|:-|:-|
| **connectionUrl** | String | OneRoster のインスタンスへの接続 URL です。 |
| **schoolsIds** | String コレクション |  同期するのには学校の sourcedIds のリスト。 |
| **プロバイダー** | String | [OneRoster 仕様](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA)で定義されているの OneRoster のサービス プロバイダーの名前です。 |
| **connectionSettings** | [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md) | OneRoster インスタンスの接続の設定です。 型[educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md)または[educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md)でなければなりません。 |
| **カスタマイズ** | [educationSynchronizationCustomizations](educationsynchronizationcustomizations.md) | 同期プロファイルを適用するオプションのカスタマイズ。|

## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationoneRosterApiDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationoneRosterApiDataProvider",
    "connectionUrl": "String",
    "providerName": "String",
    "schoolsIds": [
        "String"
    ],
    "connectionSettings": {
        "@odata.type": "#microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
        "clientId": "String",
        "clientSecret": "String",
    },
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
