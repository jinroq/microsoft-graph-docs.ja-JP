---
title: implicitGrantSettings リソースの種類
description: この web アプリケーションが OAuth 2.0 暗黙的フローを使用してトークンを要求できるかどうかを指定します。 個別のプロパティは、要求 ID とアクセストークンが暗黙的フローの一部として使用できます。 暗黙的フローを有効にするには、次のプロパティの少なくとも1つを true に設定する必要があります。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 92ba18488cc2700b565be47bac3874b6d75e1c13
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005794"
---
# <a name="implicitgrantsettings-resource-type"></a>implicitGrantSettings リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

この web アプリケーションが OAuth 2.0 暗黙的フローを使用してトークンを要求できるかどうかを指定します。 個別のプロパティは、要求 ID とアクセストークンが暗黙的フローの一部として使用できます。 暗黙的フローを有効にするには、次のプロパティの少なくとも1つを true に設定する必要があります。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------|:-----|:------------|
|enableIdTokenIssuance| Boolean | この web アプリケーションが OAuth 2.0 暗黙的フローを使用して ID トークンを要求できるかどうかを指定します。|
|enableAccessTokenIssuance| Boolean | この web アプリケーションが OAuth 2.0 暗黙的フローを使用してアクセストークンを要求できるかどうかを指定します。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.implicitGrantSettings"
}-->
```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```
