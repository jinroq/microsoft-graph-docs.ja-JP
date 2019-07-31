---
title: レポート リソースの種類
description: 複数のワークフローをサポートする Microsoft Graph API for Intune のレポートリソースについて説明します。
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c27df6cb965e4be5c186ee8bf14a65e467f538b4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010393"
---
# <a name="report-resource-type"></a>レポート リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

コンテキストに適した次の内容を返します。

- デバイス構成プロファイルの履歴レポート。
- 登録エラーレポート。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|content|Stream|レポートコンテンツ。詳細はレポートの種類によって異なります。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.report"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.report",
  "content": "<Unknown Primitive Type Edm.Stream>"
}
```



