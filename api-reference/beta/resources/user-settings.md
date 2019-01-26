---
title: 設定リソースの種類
description: '現在のユーザー設定します。 '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5812141d21a32b8ab1835a75c05cbd57ea25a3a4
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571815"
---
# <a name="settings-resource-type"></a><span data-ttu-id="04af5-103">設定リソースの種類</span><span class="sxs-lookup"><span data-stu-id="04af5-103">settings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04af5-104">現在のユーザー設定します。</span><span class="sxs-lookup"><span data-stu-id="04af5-104">The current user settings.</span></span> <span data-ttu-id="04af5-105">取得またはユーザー設定を更新する方法については、[設定を取得](../api/user-get-settings.md)および[設定の更新](../api/user-update-settings.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04af5-105">To learn how to get or update user settings, see [Get settings](../api/user-get-settings.md) and [Update settings](../api/user-update-settings.md).</span></span>

<span data-ttu-id="04af5-106">このリソースは次の内容サポートしています。</span><span class="sxs-lookup"><span data-stu-id="04af5-106">This resource supports:</span></span>

- <span data-ttu-id="04af5-107">ユーザーおよびユーザーの組織がコンテンツの検出に貢献するかどうかを確認しています。</span><span class="sxs-lookup"><span data-stu-id="04af5-107">Checking whether a user and the user's organization contribute to content discovery.</span></span>
- <span data-ttu-id="04af5-108">無効にするか、特定のユーザーに対してコンテンツの検出を有効にするとします。</span><span class="sxs-lookup"><span data-stu-id="04af5-108">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="04af5-109">Office についてのドキュメントも無効になります。</span><span class="sxs-lookup"><span data-stu-id="04af5-109">This also disables documents in Office Delve.</span></span>

## <a name="methods"></a><span data-ttu-id="04af5-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="04af5-110">Methods</span></span>
| <span data-ttu-id="04af5-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="04af5-111">Method</span></span>       | <span data-ttu-id="04af5-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="04af5-112">Return Type</span></span>  |<span data-ttu-id="04af5-113">説明</span><span class="sxs-lookup"><span data-stu-id="04af5-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="04af5-114">ユーザー設定を取得する</span><span class="sxs-lookup"><span data-stu-id="04af5-114">Get user settings</span></span>](../api/user-get-settings.md) |[<span data-ttu-id="04af5-115">設定</span><span class="sxs-lookup"><span data-stu-id="04af5-115">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="04af5-116">ユーザーと組織の設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="04af5-116">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="04af5-117">ユーザー設定の更新</span><span class="sxs-lookup"><span data-stu-id="04af5-117">Update user settings</span></span>](../api/user-update-settings.md) |[<span data-ttu-id="04af5-118">設定</span><span class="sxs-lookup"><span data-stu-id="04af5-118">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="04af5-119">ユーザーの現在の設定を更新します。</span><span class="sxs-lookup"><span data-stu-id="04af5-119">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="04af5-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04af5-120">Properties</span></span>

| <span data-ttu-id="04af5-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04af5-121">Property</span></span>     | <span data-ttu-id="04af5-122">型</span><span class="sxs-lookup"><span data-stu-id="04af5-122">Type</span></span>   |<span data-ttu-id="04af5-123">説明</span><span class="sxs-lookup"><span data-stu-id="04af5-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04af5-124">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="04af5-124">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="04af5-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="04af5-125">Boolean</span></span>|<span data-ttu-id="04af5-126">True を設定する、ユーザーの代理人アクセスを設定すると API の[トレンド分析](insights-trending.md)は無効になります。</span><span class="sxs-lookup"><span data-stu-id="04af5-126">When set to true, the delegate access to the user's [trending](insights-trending.md) API is disabled.</span></span> <span data-ttu-id="04af5-127">ユーザーの Office について true の場合、ドキュメントに設定が無効にした場合。</span><span class="sxs-lookup"><span data-stu-id="04af5-127">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="04af5-128">SharePoint ホームの候補のサイトでは、Office 365 に表示される内容との関連性を true に設定して、ビジネスのための OneDrive で検出表示が影響を受けます。</span><span class="sxs-lookup"><span data-stu-id="04af5-128">When set to true, the relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="04af5-129">ユーザーは、 [Office の説明](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout)では、この設定を制御できます。</span><span class="sxs-lookup"><span data-stu-id="04af5-129">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="04af5-130">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="04af5-130">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="04af5-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="04af5-131">Boolean</span></span>|<span data-ttu-id="04af5-132">[トレンド分析](insights-trending.md)API に代理人アクセスを制御する[組織レベルの設定](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff)が反映されます。</span><span class="sxs-lookup"><span data-stu-id="04af5-132">Reflects the [organization level setting](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](insights-trending.md) API.</span></span> <span data-ttu-id="04af5-133">場合 true の場合、組織に設定するには、Office の説明へのアクセスがありません。</span><span class="sxs-lookup"><span data-stu-id="04af5-133">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="04af5-134">候補のサイトでは、SharePoint のホームとビジネスの OneDrive で検出ビューでは、Office 365 に表示される内容との関連性は組織全体に影響を受けます。</span><span class="sxs-lookup"><span data-stu-id="04af5-134">The relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="04af5-135">この設定は読み取り専用であり、 [SharePoint 管理者センター](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US)の管理者によってのみ変更できます。</span><span class="sxs-lookup"><span data-stu-id="04af5-135">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="04af5-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="04af5-136">JSON representation</span></span>

<span data-ttu-id="04af5-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="04af5-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.userSettings"
}-->
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
