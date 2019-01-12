---
title: educationSynchronizationOAuth1ConnectionSettings リソース
description: データ プロバイダーへの接続に使用する OAuth1 がある場合は、プロファイルを設定するのにはこの接続の設定の種類を使用してください。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 80921488e1a5e0dd3e4ab4e21b2ea08e05ad9cee
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990265"
---
# <a name="educationsynchronizationoauth1connectionsettings-resource"></a>educationSynchronizationOAuth1ConnectionSettings リソース

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

データ プロバイダーへの接続に使用する OAuth1 がある場合は、プロファイルを設定するのにはこの接続の設定の種類を使用してください。

[EducationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)から派生します。

## <a name="properties"></a>プロパティ

この型では、追加のプロパティは公開されません。

## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
  "@odata.type": "#microsoft.graph.educationSynchronizationOAuth1ConnectionSettings"
}-->

```json
"connectionSettings": {
    "@odata.type": "#microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
    "clientId": "String",
    "clientSecret": "String"
}
```
