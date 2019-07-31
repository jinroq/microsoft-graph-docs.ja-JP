---
title: 履歴リソースの種類
description: Dynamics 365 Business Central のジャーナル。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 7cfc723a4370c2b30440dcd4e33b50ed066ac89b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006593"
---
# <a name="journal-resource-type"></a>履歴リソースの種類
Dynamics 365 Business Central のジャーナルを表します。

## <a name="methods"></a>メソッド

| メソッド                                            |戻り値の型|説明    |
|:--------------------------------------------------|:----------|:--------------|
|[仕訳帳を取得する](../api/dynamics-journal-get.md)      |雑誌    |ジャーナルを取得します。   |
|[仕訳帳の投稿](../api/dynamics-create-journal.md)  |雑誌    |仕訳帳を作成します。|
|[Patch ジャーナル](../api/dynamics-journal-update.md) |雑誌    |仕訳帳を更新します。|
|[仕訳帳を削除する](../api/dynamics-journal-delete.md)|none       |仕訳帳を削除します。|

## <a name="properties"></a>プロパティ
| プロパティ           | 型                  |説明                                           |
|:-------------------|:----------------------|:-----------------------------------------------------|
|id                  |GUID                   |ジャーナルの一意の ID。 編集できません。           |
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

