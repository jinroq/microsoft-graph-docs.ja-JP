---
title: リソースの種類の設定
description: '現在のユーザー設定。 '
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 433824e715940f2309619a0467179ef99ee3daec
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456934"
---
# <a name="settings-resource-type"></a><span data-ttu-id="10c60-103">リソースの種類の設定</span><span class="sxs-lookup"><span data-stu-id="10c60-103">settings resource type</span></span>

<span data-ttu-id="10c60-104">現在のユーザー設定。</span><span class="sxs-lookup"><span data-stu-id="10c60-104">The current user settings.</span></span> <span data-ttu-id="10c60-105">ユーザーの設定を更新したりする方法については、[設定](../api/user-get-settings.md) と [設定を更新する](../api/user-update-settings.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="10c60-105">To learn how to get or update user settings, see [Get settings](../api/user-get-settings.md) and [Update settings](../api/user-update-settings.md).</span></span>

<span data-ttu-id="10c60-106">このリソースは以下をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="10c60-106">This resource supports:</span></span>

- <span data-ttu-id="10c60-107">ユーザーとユーザーの組織がコンテンツの検出に貢献するかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="10c60-107">Checking whether a user and the user's organization contribute to content discovery.</span></span>
- <span data-ttu-id="10c60-108">特定のユーザーのコンテンツの検出を有効または無効にします。</span><span class="sxs-lookup"><span data-stu-id="10c60-108">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="10c60-109">Office Delve のドキュメントも無効になります。</span><span class="sxs-lookup"><span data-stu-id="10c60-109">This also disables documents in Office Delve.</span></span>

## <a name="methods"></a><span data-ttu-id="10c60-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="10c60-110">Methods</span></span>
| <span data-ttu-id="10c60-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="10c60-111">Method</span></span>       | <span data-ttu-id="10c60-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="10c60-112">Return Type</span></span>  |<span data-ttu-id="10c60-113">説明</span><span class="sxs-lookup"><span data-stu-id="10c60-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="10c60-114">[ユーザー設定の取得](../api/user-get-settings.md)</span><span class="sxs-lookup"><span data-stu-id="10c60-114">[](../api/user-get-settings.md)Get user mailbox settings</span></span> |[<span data-ttu-id="10c60-115">設定</span><span class="sxs-lookup"><span data-stu-id="10c60-115">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="10c60-116">ユーザーおよび組織の設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="10c60-116">Get the user and organization settings.</span></span> |
|<span data-ttu-id="10c60-117">[ユーザー設定を更新する](../api/user-update-settings.md)</span><span class="sxs-lookup"><span data-stu-id="10c60-117">[](../api/user-update-settings.md)Update user mailbox settings</span></span> |[<span data-ttu-id="10c60-118">設定</span><span class="sxs-lookup"><span data-stu-id="10c60-118">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="10c60-119">ユーザーの現在の設定を更新します。</span><span class="sxs-lookup"><span data-stu-id="10c60-119">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="10c60-120">Properties</span><span class="sxs-lookup"><span data-stu-id="10c60-120">Properties</span></span>

| <span data-ttu-id="10c60-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="10c60-121">Property</span></span>     | <span data-ttu-id="10c60-122">型</span><span class="sxs-lookup"><span data-stu-id="10c60-122">Type</span></span>   |<span data-ttu-id="10c60-123">説明</span><span class="sxs-lookup"><span data-stu-id="10c60-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="10c60-124">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="10c60-124">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="10c60-125">ブール値</span><span class="sxs-lookup"><span data-stu-id="10c60-125">Boolean</span></span>|<span data-ttu-id="10c60-126">ユーザーの代理人アクセスを true に設定すると、ユーザーの[トレンド](/graph/api/resources/insights-trending?view=graph-rest-beta) API は無効になります。</span><span class="sxs-lookup"><span data-stu-id="10c60-126">When set to true, the delegate access to the user's [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) API is disabled.</span></span> <span data-ttu-id="10c60-127">True に設定する場合、ユーザーの Office Delve のドキュメントは無効になります。</span><span class="sxs-lookup"><span data-stu-id="10c60-127">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="10c60-128">True に設定する場合、たとえばSharePoint Home のおすすめサイトや OneDrive for Business の Discover ビューなどの Office 365 で表示されるコンテンツの関連性にも影響が出ます。</span><span class="sxs-lookup"><span data-stu-id="10c60-128">When set to true, the relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="10c60-129">ユーザーがこの設定で [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout)を制御することができます。</span><span class="sxs-lookup"><span data-stu-id="10c60-129">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="10c60-130">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="10c60-130">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="10c60-131">ブール値</span><span class="sxs-lookup"><span data-stu-id="10c60-131">Boolean</span></span>|<span data-ttu-id="10c60-132">[組織レベルの設定](https://support.office.com/ja-JP/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff)が代理人アクセスを制御して、[トレンド](/graph/api/resources/insights-trending?view=graph-rest-beta) API へ反映します。</span><span class="sxs-lookup"><span data-stu-id="10c60-132">Reflects the [organization level setting](https://support.office.com/ja-JP/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) API.</span></span> <span data-ttu-id="10c60-133">True に設定する場合は、組織は Office Delve へアクセスすることができません。</span><span class="sxs-lookup"><span data-stu-id="10c60-133">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="10c60-134">Office 365 で表示されるコンテンツの関連性、たとえばSharePoint Home のおすすめサイトや OneDrive for Business の Discover ビューなどは、組織全体に影響が出ます。</span><span class="sxs-lookup"><span data-stu-id="10c60-134">The relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="10c60-135">この設定は読み取り専用で、[SharePoint 管理センター](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US)の管理者しか変更することができません。</span><span class="sxs-lookup"><span data-stu-id="10c60-135">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="10c60-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="10c60-136">JSON representation</span></span>

<span data-ttu-id="10c60-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="10c60-137">Here is a JSON representation of the resource.</span></span>

```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```
