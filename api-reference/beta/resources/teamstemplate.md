---
title: teamsTemplate リソースの種類
description: TeamsTemplate エンティティをについて説明します。
ms.openlocfilehash: 76b2921e884d38a57097789b1ba64df3309d141c
ms.sourcegitcommit: 12c6e82f1417022540e534ebadbd0e8d7fb5abde
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/08/2018
ms.locfileid: "27210155"
---
# <a name="teamstemplate-resource-type"></a>teamsTemplate リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

チーム テンプレートは、マイクロソフトのチームで[チーム](../resources/team.md)を作成するための青写真です。 テンプレートは、テンプレートを使用して作成された新しいチームの構造、設定、および準備する必要があるものコンテンツを指定します。 マイクロソフトは、基本テンプレートのスイートを提供していて、お客様が独自のカスタム テンプレートを保存できます。

## <a name="properties"></a>プロパティ

| プロパティ            | 種類     | 説明 |
|:------------------- |:-------- |:----------- |
| id                  | String   | テンプレートの一意の識別子です。 Null にすることはできません。 |

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTemplate",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

# <a name="see-also"></a>関連項目

- [チーム](team.md)

