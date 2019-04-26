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
# <a name="settings-resource-type"></a><span data-ttu-id="0a4eb-103">設定リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0a4eb-103">settings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a4eb-104">現在のユーザー設定。</span><span class="sxs-lookup"><span data-stu-id="0a4eb-104">The current user settings.</span></span> <span data-ttu-id="0a4eb-105">ユーザー設定を取得または更新する方法については、「設定と[更新の設定](../api/user-update-settings.md)を[取得](../api/user-get-settings.md)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0a4eb-105">To learn how to get or update user settings, see [Get settings](../api/user-get-settings.md) and [Update settings](../api/user-update-settings.md).</span></span>

<span data-ttu-id="0a4eb-106">このリソースは以下をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="0a4eb-106">This resource supports:</span></span>

- <span data-ttu-id="0a4eb-107">ユーザーとユーザーの組織がコンテンツ検出に参加しているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="0a4eb-107">Checking whether a user and the user's organization contribute to content discovery.</span></span>
- <span data-ttu-id="0a4eb-108">特定のユーザーに対してコンテンツ検出を無効または有効にします。</span><span class="sxs-lookup"><span data-stu-id="0a4eb-108">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="0a4eb-109">これにより、Office Delve のドキュメントも無効になります。</span><span class="sxs-lookup"><span data-stu-id="0a4eb-109">This also disables documents in Office Delve.</span></span>

## <a name="methods"></a><span data-ttu-id="0a4eb-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="0a4eb-110">Methods</span></span>
| <span data-ttu-id="0a4eb-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="0a4eb-111">Method</span></span>       | <span data-ttu-id="0a4eb-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0a4eb-112">Return Type</span></span>  |<span data-ttu-id="0a4eb-113">説明</span><span class="sxs-lookup"><span data-stu-id="0a4eb-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0a4eb-114">ユーザー設定を取得する</span><span class="sxs-lookup"><span data-stu-id="0a4eb-114">Get user settings</span></span>](../api/user-get-settings.md) |[<span data-ttu-id="0a4eb-115">settings</span><span class="sxs-lookup"><span data-stu-id="0a4eb-115">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="0a4eb-116">ユーザーと組織の設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="0a4eb-116">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="0a4eb-117">ユーザー設定を更新する</span><span class="sxs-lookup"><span data-stu-id="0a4eb-117">Update user settings</span></span>](../api/user-update-settings.md) |[<span data-ttu-id="0a4eb-118">settings</span><span class="sxs-lookup"><span data-stu-id="0a4eb-118">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="0a4eb-119">ユーザーの現在の設定を更新します。</span><span class="sxs-lookup"><span data-stu-id="0a4eb-119">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="0a4eb-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a4eb-120">Properties</span></span>

| <span data-ttu-id="0a4eb-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a4eb-121">Property</span></span>     | <span data-ttu-id="0a4eb-122">型</span><span class="sxs-lookup"><span data-stu-id="0a4eb-122">Type</span></span>   |<span data-ttu-id="0a4eb-123">説明</span><span class="sxs-lookup"><span data-stu-id="0a4eb-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a4eb-124">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="0a4eb-124">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="0a4eb-125">ブール値</span><span class="sxs-lookup"><span data-stu-id="0a4eb-125">Boolean</span></span>|<span data-ttu-id="0a4eb-126">true に設定されている場合、ユーザーの[傾向](insights-trending.md)API への代理人アクセスは無効になります。</span><span class="sxs-lookup"><span data-stu-id="0a4eb-126">When set to true, the delegate access to the user's [trending](insights-trending.md) API is disabled.</span></span> <span data-ttu-id="0a4eb-127">true に設定すると、ユーザーの Office Delve のドキュメントは無効になります。</span><span class="sxs-lookup"><span data-stu-id="0a4eb-127">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="0a4eb-128">true に設定すると、Office 365 に表示されるコンテンツの関連性 (SharePoint Home のおすすめサイト、OneDrive for business の検出ビューなど) が影響を受けます。</span><span class="sxs-lookup"><span data-stu-id="0a4eb-128">When set to true, the relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="0a4eb-129">ユーザーは、 [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout)でこの設定を制御できます。</span><span class="sxs-lookup"><span data-stu-id="0a4eb-129">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="0a4eb-130">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="0a4eb-130">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="0a4eb-131">ブール値</span><span class="sxs-lookup"><span data-stu-id="0a4eb-131">Boolean</span></span>|<span data-ttu-id="0a4eb-132">[傾向分析](insights-trending.md)API への代理人アクセスを制御する、[組織レベルの設定](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff)を反映します。</span><span class="sxs-lookup"><span data-stu-id="0a4eb-132">Reflects the [organization level setting](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](insights-trending.md) API.</span></span> <span data-ttu-id="0a4eb-133">true に設定すると、組織は Office Delve へのアクセス権を持ちません。</span><span class="sxs-lookup"><span data-stu-id="0a4eb-133">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="0a4eb-134">Office 365 に表示されるコンテンツの関連性 (SharePoint Home のおすすめサイト、OneDrive for business の検出ビューなど) は、組織全体で影響を受けます。</span><span class="sxs-lookup"><span data-stu-id="0a4eb-134">The relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="0a4eb-135">この設定は読み取り専用であり、 [SharePoint 管理センター](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US)の管理者のみが変更できます。</span><span class="sxs-lookup"><span data-stu-id="0a4eb-135">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0a4eb-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0a4eb-136">JSON representation</span></span>

<span data-ttu-id="0a4eb-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0a4eb-137">Here is a JSON representation of the resource.</span></span>

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
