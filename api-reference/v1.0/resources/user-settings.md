---
title: 設定リソースの種類
description: '現在のユーザー設定します。 '
ms.openlocfilehash: 291ec0b8d11a94d082534f5a890b556df89d665e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022736"
---
# <a name="settings-resource-type"></a><span data-ttu-id="d792f-103">設定リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d792f-103">settings resource type</span></span>

<span data-ttu-id="d792f-104">現在のユーザー設定します。</span><span class="sxs-lookup"><span data-stu-id="d792f-104">The current user settings.</span></span> <span data-ttu-id="d792f-105">取得またはユーザー設定を更新する方法については、[設定を取得](../api/user-get-settings.md)および[設定の更新](../api/user-update-settings.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d792f-105">To learn how to get or update user settings, see [Get settings](../api/user-get-settings.md) and [Update settings](../api/user-update-settings.md).</span></span>

<span data-ttu-id="d792f-106">このリソースは以下をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="d792f-106">This resource supports:</span></span>

- <span data-ttu-id="d792f-107">ユーザーおよびユーザーの組織がコンテンツの検出に貢献するかどうかを確認しています。</span><span class="sxs-lookup"><span data-stu-id="d792f-107">Checking whether a user and the user's organization contribute to content discovery.</span></span>
- <span data-ttu-id="d792f-108">無効にするか、特定のユーザーに対してコンテンツの検出を有効にするとします。</span><span class="sxs-lookup"><span data-stu-id="d792f-108">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="d792f-109">Office についてのドキュメントも無効になります。</span><span class="sxs-lookup"><span data-stu-id="d792f-109">This also disables documents in Office Delve.</span></span>

## <a name="methods"></a><span data-ttu-id="d792f-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="d792f-110">Methods</span></span>
| <span data-ttu-id="d792f-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="d792f-111">Method</span></span>       | <span data-ttu-id="d792f-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d792f-112">Return Type</span></span>  |<span data-ttu-id="d792f-113">説明</span><span class="sxs-lookup"><span data-stu-id="d792f-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d792f-114">ユーザー設定を取得する</span><span class="sxs-lookup"><span data-stu-id="d792f-114">Get user settings</span></span>](../api/user-get-settings.md) |[<span data-ttu-id="d792f-115">設定</span><span class="sxs-lookup"><span data-stu-id="d792f-115">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="d792f-116">ユーザーと組織の設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="d792f-116">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="d792f-117">ユーザー設定の更新</span><span class="sxs-lookup"><span data-stu-id="d792f-117">Update user settings</span></span>](../api/user-update-settings.md) |[<span data-ttu-id="d792f-118">設定</span><span class="sxs-lookup"><span data-stu-id="d792f-118">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="d792f-119">ユーザーの現在の設定を更新します。</span><span class="sxs-lookup"><span data-stu-id="d792f-119">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="d792f-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d792f-120">Properties</span></span>

| <span data-ttu-id="d792f-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d792f-121">Property</span></span>     | <span data-ttu-id="d792f-122">型</span><span class="sxs-lookup"><span data-stu-id="d792f-122">Type</span></span>   |<span data-ttu-id="d792f-123">説明</span><span class="sxs-lookup"><span data-stu-id="d792f-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d792f-124">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="d792f-124">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="d792f-125">ブール値</span><span class="sxs-lookup"><span data-stu-id="d792f-125">Boolean</span></span>|<span data-ttu-id="d792f-126">True を設定する、ユーザーの代理人アクセスを設定すると API の[トレンド分析](/graph/api/resources/insights-trending?view=graph-rest-beta)は無効になります。</span><span class="sxs-lookup"><span data-stu-id="d792f-126">When set to true, the delegate access to the user's [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) API is disabled.</span></span> <span data-ttu-id="d792f-127">ユーザーの Office について true の場合、ドキュメントに設定が無効にした場合。</span><span class="sxs-lookup"><span data-stu-id="d792f-127">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="d792f-128">SharePoint ホームの候補のサイトでは、Office 365 に表示される内容との関連性を true に設定して、ビジネスのための OneDrive で検出表示が影響を受けます。</span><span class="sxs-lookup"><span data-stu-id="d792f-128">When set to true, the relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="d792f-129">ユーザーは、 [Office の説明](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout)では、この設定を制御できます。</span><span class="sxs-lookup"><span data-stu-id="d792f-129">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="d792f-130">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="d792f-130">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="d792f-131">ブール値</span><span class="sxs-lookup"><span data-stu-id="d792f-131">Boolean</span></span>|<span data-ttu-id="d792f-132">[トレンド分析](/graph/api/resources/insights-trending?view=graph-rest-beta)API に代理人アクセスを制御する[組織レベルの設定](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff)が反映されます。</span><span class="sxs-lookup"><span data-stu-id="d792f-132">Reflects the [organization level setting](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) API.</span></span> <span data-ttu-id="d792f-133">場合 true の場合、組織に設定するには、Office の説明へのアクセスがありません。</span><span class="sxs-lookup"><span data-stu-id="d792f-133">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="d792f-134">候補のサイトでは、SharePoint のホームとビジネスの OneDrive で検出ビューでは、Office 365 に表示される内容との関連性は組織全体に影響を受けます。</span><span class="sxs-lookup"><span data-stu-id="d792f-134">The relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="d792f-135">この設定は読み取り専用であり、 [SharePoint 管理者センター](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US)の管理者によってのみ変更できます。</span><span class="sxs-lookup"><span data-stu-id="d792f-135">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="d792f-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d792f-136">JSON representation</span></span>

<span data-ttu-id="d792f-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d792f-137">Here is a JSON representation of the resource.</span></span>

```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```