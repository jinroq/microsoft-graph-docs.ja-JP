---
title: レポート リソースの種類
description: 複数のワークフローをサポートする Microsoft Graph API for Intune のレポートリソースについて説明します。
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: f94be1bcc5dfde092c6360bbdddd96d604d30a55
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939673"
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

## <a name="relationships"></a>関係
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



