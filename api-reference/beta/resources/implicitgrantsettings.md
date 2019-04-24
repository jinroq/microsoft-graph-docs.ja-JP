---
title: implicitGrantSettings リソースの種類
description: この web アプリケーションが OAuth 2.0 暗黙的フローを使用してトークンを要求できるかどうかを指定します。 個別のプロパティは、要求 ID とアクセストークンが暗黙的フローの一部として使用できます。 暗黙的フローを有効にするには、次のプロパティの少なくとも1つを true に設定する必要があります。
localization_priority: Normal
ms.openlocfilehash: 6714b9448f2e49419e41fa62822498ceaa232170
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506223"
---
# <a name="implicitgrantsettings-resource-type"></a>implicitGrantSettings リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

この web アプリケーションが OAuth 2.0 暗黙的フローを使用してトークンを要求できるかどうかを指定します。 個別のプロパティは、要求 ID とアクセストークンが暗黙的フローの一部として使用できます。 暗黙的フローを有効にするには、次のプロパティの少なくとも1つを true に設定する必要があります。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------|:-----|:------------|
|enableidtokenissuance| Boolean | この web アプリケーションが OAuth 2.0 暗黙的フローを使用して ID トークンを要求できるかどうかを指定します。|
|enableAccessTokenIssuance| Boolean | この web アプリケーションが OAuth 2.0 暗黙的フローを使用してアクセストークンを要求できるかどうかを指定します。|

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
