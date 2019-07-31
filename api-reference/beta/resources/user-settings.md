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
# <a name="settings-resource-type"></a><span data-ttu-id="99d73-103">リソースの種類の設定</span><span class="sxs-lookup"><span data-stu-id="99d73-103">settings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99d73-104">現在のユーザー設定。</span><span class="sxs-lookup"><span data-stu-id="99d73-104">The current user settings.</span></span> <span data-ttu-id="99d73-105">ユーザーの設定を更新したりする方法については、[設定](../api/user-get-settings.md) と [設定を更新する](../api/user-update-settings.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="99d73-105">To learn how to get or update user settings, see [Get settings](../api/user-get-settings.md) and [Update settings](../api/user-update-settings.md).</span></span>

<span data-ttu-id="99d73-106">このリソースは以下をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="99d73-106">This resource supports:</span></span>

- <span data-ttu-id="99d73-107">ユーザーとユーザーの組織がコンテンツの検出に貢献するかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="99d73-107">Checking whether a user and the user's organization contribute to content discovery.</span></span>
- <span data-ttu-id="99d73-108">特定のユーザーのコンテンツの検出を有効または無効にします。</span><span class="sxs-lookup"><span data-stu-id="99d73-108">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="99d73-109">Office Delve のドキュメントも無効になります。</span><span class="sxs-lookup"><span data-stu-id="99d73-109">This also disables documents in Office Delve.</span></span>

## <a name="methods"></a><span data-ttu-id="99d73-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="99d73-110">Methods</span></span>
| <span data-ttu-id="99d73-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="99d73-111">Method</span></span>       | <span data-ttu-id="99d73-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="99d73-112">Return Type</span></span>  |<span data-ttu-id="99d73-113">説明</span><span class="sxs-lookup"><span data-stu-id="99d73-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="99d73-114">ユーザー設定の取得</span><span class="sxs-lookup"><span data-stu-id="99d73-114">Get user settings</span></span>](../api/user-get-settings.md) |[<span data-ttu-id="99d73-115">設定</span><span class="sxs-lookup"><span data-stu-id="99d73-115">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="99d73-116">ユーザーおよび組織の設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="99d73-116">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="99d73-117">ユーザー設定を更新する</span><span class="sxs-lookup"><span data-stu-id="99d73-117">Update user settings</span></span>](../api/user-update-settings.md) |[<span data-ttu-id="99d73-118">設定</span><span class="sxs-lookup"><span data-stu-id="99d73-118">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="99d73-119">ユーザーの現在の設定を更新します。</span><span class="sxs-lookup"><span data-stu-id="99d73-119">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="99d73-120">Properties</span><span class="sxs-lookup"><span data-stu-id="99d73-120">Properties</span></span>

| <span data-ttu-id="99d73-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="99d73-121">Property</span></span>     | <span data-ttu-id="99d73-122">型</span><span class="sxs-lookup"><span data-stu-id="99d73-122">Type</span></span>   |<span data-ttu-id="99d73-123">説明</span><span class="sxs-lookup"><span data-stu-id="99d73-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99d73-124">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="99d73-124">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="99d73-125">ブール値</span><span class="sxs-lookup"><span data-stu-id="99d73-125">Boolean</span></span>|<span data-ttu-id="99d73-126">ユーザーの代理人アクセスを true に設定すると、ユーザーの[トレンド](insights-trending.md) API は無効になります。</span><span class="sxs-lookup"><span data-stu-id="99d73-126">When set to true, the delegate access to the user's [trending](insights-trending.md) API is disabled.</span></span> <span data-ttu-id="99d73-127">True に設定する場合、ユーザーの Office Delve のドキュメントは無効になります。</span><span class="sxs-lookup"><span data-stu-id="99d73-127">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="99d73-128">True に設定する場合、たとえばSharePoint Home のおすすめサイトや OneDrive for Business の Discover ビューなどの Office 365 で表示されるコンテンツの関連性にも影響が出ます。</span><span class="sxs-lookup"><span data-stu-id="99d73-128">When set to true, the relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="99d73-129">ユーザーがこの設定で [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout)を制御することができます。</span><span class="sxs-lookup"><span data-stu-id="99d73-129">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="99d73-130">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="99d73-130">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="99d73-131">ブール値</span><span class="sxs-lookup"><span data-stu-id="99d73-131">Boolean</span></span>|<span data-ttu-id="99d73-132">[組織レベルの設定](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff)が代理人アクセスを制御して、[トレンド](insights-trending.md) API へ反映します。</span><span class="sxs-lookup"><span data-stu-id="99d73-132">Reflects the [organization level setting](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](insights-trending.md) API.</span></span> <span data-ttu-id="99d73-133">True に設定する場合は、組織は Office Delve へアクセスすることができません。</span><span class="sxs-lookup"><span data-stu-id="99d73-133">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="99d73-134">Office 365 で表示されるコンテンツの関連性、たとえばSharePoint Home のおすすめサイトや OneDrive for Business の Discover ビューなどは、組織全体に影響が出ます。</span><span class="sxs-lookup"><span data-stu-id="99d73-134">The relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="99d73-135">この設定は読み取り専用で、[SharePoint 管理センター](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US)の管理者しか変更することができません。</span><span class="sxs-lookup"><span data-stu-id="99d73-135">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="99d73-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="99d73-136">JSON representation</span></span>

<span data-ttu-id="99d73-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="99d73-137">Here is a JSON representation of the resource.</span></span>
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
