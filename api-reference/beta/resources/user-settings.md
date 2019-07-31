---
title: リソースの種類の設定
description: '現在のユーザー設定。 '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3f79bdc747c5862dd0b2bcf9b2a7dc42b4dd5a17
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007552"
---
# <a name="settings-resource-type"></a>リソースの種類の設定

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

現在のユーザー設定。 ユーザーの設定を更新したりする方法については、[設定](../api/user-get-settings.md) と [設定を更新する](../api/user-update-settings.md)を参照してください。

このリソースは以下をサポートしています。

- ユーザーとユーザーの組織がコンテンツの検出に貢献するかどうかを確認します。
- 特定のユーザーのコンテンツの検出を有効または無効にします。 Office Delve のドキュメントも無効になります。

## <a name="methods"></a>メソッド
| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[ユーザー設定の取得](../api/user-get-settings.md) |[設定](../resources/user-settings.md)| ユーザーおよび組織の設定を取得します。 |
|[ユーザー設定を更新する](../api/user-update-settings.md) |[設定](../resources/user-settings.md)| ユーザーの現在の設定を更新します。 |

## <a name="properties"></a>Properties

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|contributionToContentDiscoveryDisabled|ブール値|ユーザーの代理人アクセスを true に設定すると、ユーザーの[トレンド](insights-trending.md) API は無効になります。 True に設定する場合、ユーザーの Office Delve のドキュメントは無効になります。 True に設定する場合、たとえばSharePoint Home のおすすめサイトや OneDrive for Business の Discover ビューなどの Office 365 で表示されるコンテンツの関連性にも影響が出ます。 ユーザーがこの設定で [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout)を制御することができます。 |
|contributionToContentDiscoveryAsOrganizationDisabled|ブール値|[組織レベルの設定](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff)が代理人アクセスを制御して、[トレンド](insights-trending.md) API へ反映します。 True に設定する場合は、組織は Office Delve へアクセスすることができません。 Office 365 で表示されるコンテンツの関連性、たとえばSharePoint Home のおすすめサイトや OneDrive for Business の Discover ビューなどは、組織全体に影響が出ます。 この設定は読み取り専用で、[SharePoint 管理センター](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US)の管理者しか変更することができません。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userSettings"
}-->
```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```
