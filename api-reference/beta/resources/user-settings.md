---
title: 設定リソースの種類
description: '現在のユーザー設定。 '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 208d232af609f92d5924267ae26831b9929e357a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554269"
---
# <a name="settings-resource-type"></a>設定リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

現在のユーザー設定。 ユーザー設定を取得または更新する方法については、「設定と[更新の設定](../api/user-update-settings.md)を[取得](../api/user-get-settings.md)する」を参照してください。

このリソースは以下をサポートしています。

- ユーザーとユーザーの組織がコンテンツ検出に参加しているかどうかを確認します。
- 特定のユーザーに対してコンテンツ検出を無効または有効にします。 これにより、Office Delve のドキュメントも無効になります。

## <a name="methods"></a>メソッド
| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[ユーザー設定を取得する](../api/user-get-settings.md) |[settings](../resources/user-settings.md)| ユーザーと組織の設定を取得します。 |
|[ユーザー設定を更新する](../api/user-update-settings.md) |[settings](../resources/user-settings.md)| ユーザーの現在の設定を更新します。 |

## <a name="properties"></a>プロパティ

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|contributionToContentDiscoveryDisabled|ブール値|true に設定されている場合、ユーザーの[傾向](insights-trending.md)API への代理人アクセスは無効になります。 true に設定すると、ユーザーの Office Delve のドキュメントは無効になります。 true に設定すると、Office 365 に表示されるコンテンツの関連性 (SharePoint Home のおすすめサイト、OneDrive for business の検出ビューなど) が影響を受けます。 ユーザーは、 [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout)でこの設定を制御できます。 |
|contributionToContentDiscoveryAsOrganizationDisabled|ブール値|[傾向分析](insights-trending.md)API への代理人アクセスを制御する、[組織レベルの設定](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff)を反映します。 true に設定すると、組織は Office Delve へのアクセス権を持ちません。 Office 365 に表示されるコンテンツの関連性 (SharePoint Home のおすすめサイト、OneDrive for business の検出ビューなど) は、組織全体で影響を受けます。 この設定は読み取り専用であり、 [SharePoint 管理センター](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US)の管理者のみが変更できます。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/user-settings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
