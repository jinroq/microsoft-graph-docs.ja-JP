---
title: implicitGrantSettings リソースの種類
description: この web アプリケーションが OAuth 2.0 暗黙的フローを使用してトークンを要求できるかどうかを指定します。 個別のプロパティは、要求 ID とアクセストークンが暗黙的フローの一部として使用できます。 暗黙的フローを有効にするには、次のプロパティの少なくとも1つを true に設定する必要があります。
localization_priority: Normal
ms.openlocfilehash: 1026f3b97a3305dff7a715fae000ab9695ac8e9d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333611"
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
