---
title: 設定リソースの種類
description: '現在のユーザー設定します。 '
author: dkershaw10
ms.openlocfilehash: 81a89d726374cb9640e163d13f10825390e91c23
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316640"
---
# <a name="settings-resource-type"></a><span data-ttu-id="cfbc9-103">設定リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cfbc9-103">settings resource type</span></span>

> <span data-ttu-id="cfbc9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cfbc9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cfbc9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cfbc9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cfbc9-106">現在のユーザー設定します。</span><span class="sxs-lookup"><span data-stu-id="cfbc9-106">The current user settings.</span></span> <span data-ttu-id="cfbc9-107">取得またはユーザー設定を更新する方法については、[設定を取得](../api/user-get-settings.md)および[設定の更新](../api/user-update-settings.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cfbc9-107">To learn how to get or update user settings, see [Get settings](../api/user-get-settings.md) and [Update settings](../api/user-update-settings.md).</span></span>

<span data-ttu-id="cfbc9-108">このリソースは以下をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="cfbc9-108">This resource supports:</span></span>

- <span data-ttu-id="cfbc9-109">ユーザーおよびユーザーの組織がコンテンツの検出に貢献するかどうかを確認しています。</span><span class="sxs-lookup"><span data-stu-id="cfbc9-109">Checking whether a user and the user's organization contribute to content discovery.</span></span>
- <span data-ttu-id="cfbc9-110">無効にするか、特定のユーザーに対してコンテンツの検出を有効にするとします。</span><span class="sxs-lookup"><span data-stu-id="cfbc9-110">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="cfbc9-111">Office についてのドキュメントも無効になります。</span><span class="sxs-lookup"><span data-stu-id="cfbc9-111">This also disables documents in Office Delve.</span></span>

## <a name="methods"></a><span data-ttu-id="cfbc9-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="cfbc9-112">Methods</span></span>
| <span data-ttu-id="cfbc9-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="cfbc9-113">Method</span></span>       | <span data-ttu-id="cfbc9-114">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cfbc9-114">Return Type</span></span>  |<span data-ttu-id="cfbc9-115">説明</span><span class="sxs-lookup"><span data-stu-id="cfbc9-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cfbc9-116">ユーザー設定を取得する</span><span class="sxs-lookup"><span data-stu-id="cfbc9-116">Get user settings</span></span>](../api/user-get-settings.md) |[<span data-ttu-id="cfbc9-117">設定</span><span class="sxs-lookup"><span data-stu-id="cfbc9-117">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="cfbc9-118">ユーザーと組織の設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="cfbc9-118">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="cfbc9-119">ユーザー設定の更新</span><span class="sxs-lookup"><span data-stu-id="cfbc9-119">Update user settings</span></span>](../api/user-update-settings.md) |[<span data-ttu-id="cfbc9-120">設定</span><span class="sxs-lookup"><span data-stu-id="cfbc9-120">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="cfbc9-121">ユーザーの現在の設定を更新します。</span><span class="sxs-lookup"><span data-stu-id="cfbc9-121">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="cfbc9-122">Properties</span><span class="sxs-lookup"><span data-stu-id="cfbc9-122">Properties</span></span>

| <span data-ttu-id="cfbc9-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cfbc9-123">Property</span></span>     | <span data-ttu-id="cfbc9-124">種類</span><span class="sxs-lookup"><span data-stu-id="cfbc9-124">Type</span></span>   |<span data-ttu-id="cfbc9-125">説明</span><span class="sxs-lookup"><span data-stu-id="cfbc9-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cfbc9-126">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="cfbc9-126">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="cfbc9-127">ブール型</span><span class="sxs-lookup"><span data-stu-id="cfbc9-127">Boolean</span></span>|<span data-ttu-id="cfbc9-128">True を設定する、ユーザーの代理人アクセスを設定すると API の[トレンド分析](insights-trending.md)は無効になります。</span><span class="sxs-lookup"><span data-stu-id="cfbc9-128">When set to true, the delegate access to the user's [trending](insights-trending.md) API is disabled.</span></span> <span data-ttu-id="cfbc9-129">ユーザーの Office について true の場合、ドキュメントに設定が無効にした場合。</span><span class="sxs-lookup"><span data-stu-id="cfbc9-129">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="cfbc9-130">SharePoint ホームの候補のサイトでは、Office 365 に表示される内容との関連性を true に設定して、ビジネスのための OneDrive で検出表示が影響を受けます。</span><span class="sxs-lookup"><span data-stu-id="cfbc9-130">When set to true, the relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="cfbc9-131">ユーザーは、 [Office の説明](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout)では、この設定を制御できます。</span><span class="sxs-lookup"><span data-stu-id="cfbc9-131">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="cfbc9-132">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="cfbc9-132">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="cfbc9-133">ブール型</span><span class="sxs-lookup"><span data-stu-id="cfbc9-133">Boolean</span></span>|<span data-ttu-id="cfbc9-134">[トレンド分析](insights-trending.md)API に代理人アクセスを制御する[組織レベルの設定](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff)が反映されます。</span><span class="sxs-lookup"><span data-stu-id="cfbc9-134">Reflects the [organization level setting](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](insights-trending.md) API.</span></span> <span data-ttu-id="cfbc9-135">場合 true の場合、組織に設定するには、Office の説明へのアクセスがありません。</span><span class="sxs-lookup"><span data-stu-id="cfbc9-135">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="cfbc9-136">候補のサイトでは、SharePoint のホームとビジネスの OneDrive で検出ビューでは、Office 365 に表示される内容との関連性は組織全体に影響を受けます。</span><span class="sxs-lookup"><span data-stu-id="cfbc9-136">The relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="cfbc9-137">この設定は読み取り専用であり、 [SharePoint 管理者センター](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US)の管理者によってのみ変更できます。</span><span class="sxs-lookup"><span data-stu-id="cfbc9-137">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cfbc9-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cfbc9-138">JSON representation</span></span>

<span data-ttu-id="cfbc9-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cfbc9-139">Here is a JSON representation of the resource.</span></span>

```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```