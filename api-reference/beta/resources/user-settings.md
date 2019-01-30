---
title: 設定リソースの種類
description: '現在のユーザー設定します。 '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 208d232af609f92d5924267ae26831b9929e357a
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640512"
---
# <a name="settings-resource-type"></a>設定リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

現在のユーザー設定します。 取得またはユーザー設定を更新する方法については、[設定を取得](../api/user-get-settings.md)および[設定の更新](../api/user-update-settings.md)を参照してください。

このリソースは以下をサポートしています。

- ユーザーおよびユーザーの組織がコンテンツの検出に貢献するかどうかを確認しています。
- 無効にするか、特定のユーザーに対してコンテンツの検出を有効にするとします。 Office についてのドキュメントも無効になります。

## <a name="methods"></a>メソッド
| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[ユーザー設定を取得する](../api/user-get-settings.md) |[設定](../resources/user-settings.md)| ユーザーと組織の設定を取得します。 |
|[ユーザー設定の更新](../api/user-update-settings.md) |[設定](../resources/user-settings.md)| ユーザーの現在の設定を更新します。 |

## <a name="properties"></a>プロパティ

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|contributionToContentDiscoveryDisabled|Boolean|True を設定する、ユーザーの代理人アクセスを設定すると API の[トレンド分析](insights-trending.md)は無効になります。 ユーザーの Office について true の場合、ドキュメントに設定が無効にした場合。 SharePoint ホームの候補のサイトでは、Office 365 に表示される内容との関連性を true に設定して、ビジネスのための OneDrive で検出表示が影響を受けます。 ユーザーは、 [Office の説明](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout)では、この設定を制御できます。 |
|contributionToContentDiscoveryAsOrganizationDisabled|Boolean|[トレンド分析](insights-trending.md)API に代理人アクセスを制御する[組織レベルの設定](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff)が反映されます。 場合 true の場合、組織に設定するには、Office の説明へのアクセスがありません。 候補のサイトでは、SharePoint のホームとビジネスの OneDrive で検出ビューでは、Office 365 に表示される内容との関連性は組織全体に影響を受けます。 この設定は読み取り専用であり、 [SharePoint 管理者センター](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US)の管理者によってのみ変更できます。|

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
