---
title: 履歴リソースの種類
description: Dynamics 365 Business Central のジャーナル。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: bef5008bbacb1729f48758b228e55a3f6adc2af0
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365473"
---
# <a name="journal-resource-type"></a>履歴リソースの種類
Dynamics 365 Business Central のジャーナルを表します。

## <a name="methods"></a>メソッド

| メソッド                                            |戻り値の型|説明    |
|:--------------------------------------------------|:----------|:--------------|
|[ジャーナルを取得する](../api/dynamics-journal-get.md)      |雑誌    |ジャーナルを取得します。   |
|[仕訳帳の投稿](../api/dynamics-create-journal.md)  |雑誌    |仕訳帳を作成します。|
|[Patch ジャーナル](../api/dynamics-journal-update.md) |雑誌    |仕訳帳を更新します。|
|[ジャーナルの削除](../api/dynamics-journal-delete.md)|none       |仕訳帳を削除します。|

## <a name="properties"></a>プロパティ
| プロパティ           | 型                  |説明                                           |
|:-------------------|:----------------------|:-----------------------------------------------------|
|ID                  |GUID                   |ジャーナルの一意の ID。 編集不可。           |
|code                |文字列、最大サイズ10| ジャーナルのコード。                             |
|displayName         |文字列、最大サイズ50| 仕訳帳の表示名。                     |
|lastModifiedDateTime|datetime               |ジャーナルが変更された最後の datetime。 読み取り専用です。|

## <a name="bound-actions"></a>バインドされたアクション
ジャーナルリソースの種類は、と呼ば`post`れる、対応する一般的なジャーナルバッチを投稿するバインドアクションを提供します。

次の例に、一般的なジャーナルバッチの投稿を示します。  
`POST https://graph.microsoft.com/beta/financials/companies{id}/journals{id}/post`.

応答にはコンテンツがありません。応答コードは204です。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}
```

