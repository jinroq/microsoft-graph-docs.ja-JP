---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 85def7dd812d2046e02f814cf63e9f82b28d2781
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919688"
---
# <a name="driverecipient-resource"></a>DriveRecipient リソース

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**DriveRecipient** リソースは、[出席依頼](../api/driveitem-invite.md)アクションを使用して共有する個人、グループ、または他の受信者を表します。

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

| プロパティ名 | Type   | 説明                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| email         | String | 受信者が関連付けられた電子メール アドレスを設定している場合は、受信者の電子メール アドレスです。                  |
| alias         | String | 電子メール アドレスが使用できない場合は、ドメイン オブジェクトのエイリアス (セキュリティ グループなど) です。 |
| objectId      | String | ディレクトリ内の受信者の一意識別子。                                               |

## <a name="remarks"></a>注釈

[出席依頼](../api/driveitem-invite.md)を使用して、アクセス許可を追加する場合は、DriveRecipient で **email**、**alias**、または **objectId** を指定できます。これらの値のうち 1 つのみが必要です。

<!-- {
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients"
} -->
