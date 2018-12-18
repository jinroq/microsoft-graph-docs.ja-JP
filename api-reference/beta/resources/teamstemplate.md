---
title: teamsTemplate リソースの種類
description: TeamsTemplate エンティティをについて説明します。
author: nkramer
ms.openlocfilehash: b4e32448f864048fdcb54dc001b21b262df2bba3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327714"
---
# <a name="teamstemplate-resource-type"></a>teamsTemplate リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

チーム テンプレートは、マイクロソフトのチームで[チーム](../resources/team.md)を作成するための青写真です。 テンプレートは、テンプレートを使用して作成された新しいチームの構造、設定、および準備する必要があるものコンテンツを指定します。 マイクロソフトは、基本テンプレートのスイートを提供していて、お客様が独自のカスタム テンプレートを保存できます。

## <a name="properties"></a>Properties

| プロパティ            | 種類     | 説明 |
|:------------------- |:-------- |:----------- |
| ID                  | String   | テンプレートの一意の識別子です。 Null にすることはできません。 |

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

