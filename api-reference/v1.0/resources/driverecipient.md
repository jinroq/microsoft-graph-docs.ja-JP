---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveRecipient
ms.openlocfilehash: 53f6a5559cb90142a88b839a996cb2eedfd1037a
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="driverecipient-resource"></a>DriveRecipient リソース

**DriveRecipient** リソースは、[出席依頼](../api/driveitem_invite.md)アクションを使用して共有する個人、グループ、または他の受信者を表します。

## <a name="json-representation"></a>JSON 表記

<!-- { 
  "blockType": "resource", 
  "@odata.type": "microsoft.graph.driveRecipient", 
  "optionalProperties": ["alias", "objectId", "email"] } -->
```json
{
  "email": "string",
  "alias": "string",
  "objectId": "string",
}
```

## <a name="properties"></a>プロパティ
受信者のリソースには、これらのプロパティがあります。

| プロパティ名 | 種類   | 説明                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| email         | String | 受信者が関連付けられた電子メール アドレスを設定している場合は、受信者の電子メール アドレスです。                  |
| alias         | String | 電子メール アドレスが使用できない場合は、ドメイン オブジェクトのエイリアス (セキュリティ グループなど) です。 |
| objectId      | String | ディレクトリ内の受信者の一意識別子。                                               |

## <a name="remarks"></a>注釈

[出席依頼](../api/driveitem_invite.md)を使用して、アクセス許可を追加する場合は、DriveRecipient で **email**、**alias**、または **objectId** を指定できます。
これらの値のうち 1 つのみが必要です。

<!-- {
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients"
} -->
