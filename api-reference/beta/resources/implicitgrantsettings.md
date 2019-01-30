---
title: implicitGrantSettings リソースの種類
description: この web アプリケーションが、OAuth 2.0 の暗黙的なフローを使用してトークンを要求できるかどうかを指定します。 暗黙の流れの一部として、ID とアクセス トークンを要求する別のプロパティを利用できます。 暗黙のフローを有効にするには、次のプロパティの少なくとも 1 つ設定する必要がある true に設定します。
localization_priority: Normal
ms.openlocfilehash: 6714b9448f2e49419e41fa62822498ceaa232170
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642766"
---
# <a name="implicitgrantsettings-resource-type"></a>implicitGrantSettings リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

この web アプリケーションが、OAuth 2.0 の暗黙的なフローを使用してトークンを要求できるかどうかを指定します。 暗黙の流れの一部として、ID とアクセス トークンを要求する別のプロパティを利用できます。 暗黙のフローを有効にするには、次のプロパティの少なくとも 1 つ設定する必要がある true に設定します。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------|:-----|:------------|
|enableIdTokenIssuance| Boolean | この web アプリケーションが、OAuth 2.0 の暗黙的なフローを使用して ID トークンを要求できるかどうかを指定します。|
|enableAccessTokenIssuance| Boolean | この web アプリケーションで、OAuth 2.0 の暗黙的なフローを使用してアクセス トークンを要求できるかどうかを指定します。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/implicitgrantsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
