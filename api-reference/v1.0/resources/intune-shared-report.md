---
title: レポート リソースの種類
description: ワークフローによって異なるレポート。デバイス構成プロファイル履歴または登録の失敗のいずれかです。
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9348abb1b63f4c83604213ce1f9ad0a521a85c05
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036877"
---
# <a name="report-resource-type"></a>レポート リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

ワークフローによって異なるレポート。デバイス構成プロファイル履歴または登録の失敗のいずれかです。

## <a name="properties"></a>プロパティ

|プロパティ|型|説明|
|:---|:---|:---|
|content|Stream|まだ文書化されていません|

## <a name="relationships"></a>リレーションシップ

なし

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.report"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.report",
  "content": "<Unknown Primitive Type Edm.Stream>"
}
```
