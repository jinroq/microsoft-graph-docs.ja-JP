---
title: レポート リソースの種類
description: 複数のワークフローをサポートする Microsoft Graph API for Intune のレポートリソースについて説明します。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: f523f6df0b8b90cb6649ac81f1e433d6df227aea
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534816"
---
# <a name="report-resource-type"></a>レポート リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

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



