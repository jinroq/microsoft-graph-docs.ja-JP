---
title: レポート リソースの種類
description: ワークフローによって異なるレポート。デバイス構成プロファイル履歴または登録の失敗のいずれかです。
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: ad95fa9ef21a6fbf80ddd8265b5bac2e72c1825b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523778"
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
