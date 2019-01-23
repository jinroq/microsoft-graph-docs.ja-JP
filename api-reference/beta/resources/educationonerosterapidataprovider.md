---
title: educationOneRosterApiDataProvider リソース
description: OneRoster API は、入力ソースとして使用するときに、学校のデータの同期プロファイルを設定するために使用します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ccfb74cdac64a147adb8ed7d3a0ad4b3fa3c83cd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425989"
---
# <a name="educationonerosterapidataprovider-resource"></a>educationOneRosterApiDataProvider リソース

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

[OneRoster API](https://www.imsglobal.org/activity/onerosterlis)は、入力ソースとして使用するときに、学校のデータの同期プロファイルを設定するために使用します。

[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)から派生します。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **connectionUrl** | String | OneRoster のインスタンスへの接続 URL です。 |
| **schoolsIds** | String コレクション |  同期するのには学校の sourcedIds のリスト。 |
| **プロバイダー** | String | [OneRoster 仕様](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA)で定義されているの OneRoster のサービス プロバイダーの名前です。 |
| **connectionSettings** | [microsoft.graph.educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md) | OneRoster インスタンスの接続の設定です。 型[microsoft.graph.educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md)または[microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md)でなければなりません。 |
| **カスタマイズ** | [microsoft.graph.educationSynchronizationCustomizations](educationsynchronizationcustomizations.md) | 同期プロファイルを適用するオプションのカスタマイズ。|

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
