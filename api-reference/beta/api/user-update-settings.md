---
title: 設定の更新
description: '設定オブジェクトのプロパティを更新します。 '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8f538d298f71ad7ef537988a29bae812015566ec
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913227"
---
# <a name="update-settings"></a><span data-ttu-id="7e17d-103">設定の更新</span><span class="sxs-lookup"><span data-stu-id="7e17d-103">Update settings</span></span>

> <span data-ttu-id="7e17d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7e17d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7e17d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e17d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7e17d-106">[設定](../resources/user-settings.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7e17d-106">Update the properties of the [settings](../resources/user-settings.md) object.</span></span> <span data-ttu-id="7e17d-107">同じ組織内のユーザーは、優先順位または組織のポリシーに基づいて、異なる設定を持つことができます。</span><span class="sxs-lookup"><span data-stu-id="7e17d-107">Users in the same organization can have different settings based on their preference or on the organization policies.</span></span> <span data-ttu-id="7e17d-108">ユーザーの現在の設定を取得、[現在のユーザー設定](user-get-settings.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7e17d-108">To get the user current settings, see [current user settings](user-get-settings.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="7e17d-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7e17d-109">Permissions</span></span>

<span data-ttu-id="7e17d-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7e17d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e17d-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7e17d-112">Permission type</span></span>      | <span data-ttu-id="7e17d-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7e17d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e17d-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7e17d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7e17d-115">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e17d-115">User.ReadWrite, User.ReadWrite.All</span></span>   |
|<span data-ttu-id="7e17d-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7e17d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e17d-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e17d-117">Not supported.</span></span>    |
|<span data-ttu-id="7e17d-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7e17d-118">Application</span></span> | <span data-ttu-id="7e17d-119">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e17d-119">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e17d-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7e17d-120">HTTP request</span></span>

```http
PATCH https://graph.microsoft.com/beta/me/settings
```

<span data-ttu-id="7e17d-121">'UserPrincipalName' は、ユーザー、または User.ReadWrite.All のアクセス許可を持つユーザーがアクセス可能なや、ユーザー id が要求されます。</span><span class="sxs-lookup"><span data-stu-id="7e17d-121">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="7e17d-122">詳細については、[アクセス許可](/graph/permissions-reference)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7e17d-122">To learn more, see [Permissions](/graph/permissions-reference).</span></span> 

```http
PATCH https://graph.microsoft.com/beta/users/{id | userPrincipalName}/settings/
```

## <a name="request-headers"></a><span data-ttu-id="7e17d-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7e17d-123">Request headers</span></span>

| <span data-ttu-id="7e17d-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7e17d-124">Header</span></span>       | <span data-ttu-id="7e17d-125">値</span><span class="sxs-lookup"><span data-stu-id="7e17d-125">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="7e17d-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e17d-126">Authorization</span></span>  | <span data-ttu-id="7e17d-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7e17d-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7e17d-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7e17d-129">Content-Type</span></span>  | <span data-ttu-id="7e17d-130">application/json</span><span class="sxs-lookup"><span data-stu-id="7e17d-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7e17d-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="7e17d-131">Request body</span></span>

<span data-ttu-id="7e17d-p106">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="7e17d-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7e17d-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e17d-135">Property</span></span>     | <span data-ttu-id="7e17d-136">種類</span><span class="sxs-lookup"><span data-stu-id="7e17d-136">Type</span></span>   |<span data-ttu-id="7e17d-137">説明</span><span class="sxs-lookup"><span data-stu-id="7e17d-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e17d-138">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="7e17d-138">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="7e17d-139">ブール型</span><span class="sxs-lookup"><span data-stu-id="7e17d-139">Boolean</span></span>|<span data-ttu-id="7e17d-140">True を設定するには、 [Trending](../resources/insights-trending.md) API およびユーザーの Office についてのドキュメントへのアクセスを無効にする代理人へのアクセスは無効にします。</span><span class="sxs-lookup"><span data-stu-id="7e17d-140">Set to true do disable delegate access to the [Trending](../resources/insights-trending.md) API and to disable access to documents in Office Delve for the user.</span></span> <span data-ttu-id="7e17d-141">Office 365 に表示されるコンテンツの関連性に影響を与えるも true に設定 - 候補のサイトでは、SharePoint のホームとビジネスの OneDrive の検索ビューの関連性の低い結果を表示するたとえば、します。</span><span class="sxs-lookup"><span data-stu-id="7e17d-141">Setting to true also affects the relevance of the content displayed in Office 365 - for example, Suggested sites in SharePoint Home and the Discover view in OneDrive for Business show less relevant results.</span></span> <span data-ttu-id="7e17d-142">この設定は、 [Office の説明](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout)でコントロールの状態を反映しています。</span><span class="sxs-lookup"><span data-stu-id="7e17d-142">This setting reflects the control state in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span>|

## <a name="example"></a><span data-ttu-id="7e17d-143">例</span><span class="sxs-lookup"><span data-stu-id="7e17d-143">Example</span></span> 

##### <a name="request"></a><span data-ttu-id="7e17d-144">要求</span><span class="sxs-lookup"><span data-stu-id="7e17d-144">Request</span></span>

<span data-ttu-id="7e17d-145">Delve のユーザーを無効にし、組織全体のコンテンツの関連性に関する彼の貢献度を無効にする方法について、例の要求は、ここで。</span><span class="sxs-lookup"><span data-stu-id="7e17d-145">Here is an example request on how to opt-out a user from Delve and disable his contribution on content relevancy for the whole organization.</span></span>

```http
PATCH https://graph.microsoft.com/beta/me/settings
Content-type: application/json
Content-length: 37

{
  "contributionToContentDiscoveryDisabled": true
}
```

##### <a name="response"></a><span data-ttu-id="7e17d-146">応答</span><span class="sxs-lookup"><span data-stu-id="7e17d-146">Response</span></span>

<span data-ttu-id="7e17d-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7e17d-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```

#### <a name="batch-request"></a><span data-ttu-id="7e17d-150">バッチ要求</span><span class="sxs-lookup"><span data-stu-id="7e17d-150">Batch request</span></span>

<span data-ttu-id="7e17d-151">Delve から複数のユーザーを無効にし、バッチ要求を組織全体でのコンテンツの関連性のような貢献を無効にすることもできます。</span><span class="sxs-lookup"><span data-stu-id="7e17d-151">It's also possible to opt-out multiple users from Delve and disable their contribution on content relevancy for the whole organization through a batch request.</span></span>
<span data-ttu-id="7e17d-152">詳細については、 [JSON のバッチ処理](/graph/json-batching)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7e17d-152">To learn more, see [JSON batching](/graph/json-batching).</span></span>

<span data-ttu-id="7e17d-153">**重要**: だけで、[組織の管理](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US)役割グループのメンバーは、複数のユーザーを更新できます。</span><span class="sxs-lookup"><span data-stu-id="7e17d-153">**Important**: Only members of the [Organization Management](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) role group can update multiple users.</span></span> 


