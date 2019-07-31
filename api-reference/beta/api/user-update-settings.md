---
title: 設定を更新する
description: 'Settings オブジェクトのプロパティを更新します。 '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a6b5903e08cfef70bace2f2dc6f2692e54fd7961
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35996099"
---
# <a name="update-settings"></a><span data-ttu-id="e48f8-103">設定を更新する</span><span class="sxs-lookup"><span data-stu-id="e48f8-103">Update settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e48f8-104">[Settings](../resources/user-settings.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e48f8-104">Update the properties of the [settings](../resources/user-settings.md) object.</span></span> <span data-ttu-id="e48f8-105">同じ組織内のユーザーは、そのユーザーの好みまたは組織のポリシーに基づいて設定を変えることができます。</span><span class="sxs-lookup"><span data-stu-id="e48f8-105">Users in the same organization can have different settings based on their preference or on the organization policies.</span></span> <span data-ttu-id="e48f8-106">ユーザーの現在の設定を取得するには、「[現在のユーザーの設定](user-get-settings.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e48f8-106">To get the user current settings, see [current user settings](user-get-settings.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="e48f8-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e48f8-107">Permissions</span></span>

<span data-ttu-id="e48f8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e48f8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e48f8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e48f8-110">Permission type</span></span>      | <span data-ttu-id="e48f8-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e48f8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e48f8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e48f8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e48f8-113">ユーザー読み取り/書き込みユーザー。</span><span class="sxs-lookup"><span data-stu-id="e48f8-113">User.ReadWrite, User.ReadWrite.All</span></span>   |
|<span data-ttu-id="e48f8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e48f8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e48f8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e48f8-115">Not supported.</span></span>    |
|<span data-ttu-id="e48f8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e48f8-116">Application</span></span> | <span data-ttu-id="e48f8-117">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e48f8-117">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e48f8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e48f8-118">HTTP request</span></span>

```http
PATCH /me/settings
```

<span data-ttu-id="e48f8-119">「user id」または「userPrincipalName」を持つリクエストは、ユーザーまたは User.ReadWrite.All 権限を持つユーザーのみがアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="e48f8-119">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="e48f8-120">詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e48f8-120">To learn more, see [Permissions](/graph/permissions-reference).</span></span> 

```http
PATCH /users/{id | userPrincipalName}/settings/
```

## <a name="request-headers"></a><span data-ttu-id="e48f8-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e48f8-121">Request headers</span></span>

| <span data-ttu-id="e48f8-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e48f8-122">Header</span></span>       | <span data-ttu-id="e48f8-123">値</span><span class="sxs-lookup"><span data-stu-id="e48f8-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="e48f8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e48f8-124">Authorization</span></span>  | <span data-ttu-id="e48f8-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e48f8-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e48f8-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e48f8-127">Content-Type</span></span>  | <span data-ttu-id="e48f8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e48f8-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e48f8-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="e48f8-129">Request body</span></span>

<span data-ttu-id="e48f8-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="e48f8-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e48f8-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e48f8-133">Property</span></span>     | <span data-ttu-id="e48f8-134">型</span><span class="sxs-lookup"><span data-stu-id="e48f8-134">Type</span></span>   |<span data-ttu-id="e48f8-135">説明</span><span class="sxs-lookup"><span data-stu-id="e48f8-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e48f8-136">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="e48f8-136">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="e48f8-137">ブール値</span><span class="sxs-lookup"><span data-stu-id="e48f8-137">Boolean</span></span>|<span data-ttu-id="e48f8-138">True に設定[トレンド分析](../resources/insights-trending.md)API への代理人アクセスを無効にし、ユーザーの Office Delve でドキュメントへのアクセスを無効にします。</span><span class="sxs-lookup"><span data-stu-id="e48f8-138">Set to true do disable delegate access to the [Trending](../resources/insights-trending.md) API and to disable access to documents in Office Delve for the user.</span></span> <span data-ttu-id="e48f8-139">True に設定すると、Office 365 に表示されるコンテンツの関連性にも影響します。たとえば、SharePoint ホームのおすすめサイト、OneDrive for Business の検出ビューには関連性の低い検索結果が表示されます。</span><span class="sxs-lookup"><span data-stu-id="e48f8-139">Setting to true also affects the relevance of the content displayed in Office 365 - for example, Suggested sites in SharePoint Home and the Discover view in OneDrive for Business show less relevant results.</span></span> <span data-ttu-id="e48f8-140">この設定は、 [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout)のコントロールの状態を反映します。</span><span class="sxs-lookup"><span data-stu-id="e48f8-140">This setting reflects the control state in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span>|

## <a name="example"></a><span data-ttu-id="e48f8-141">例</span><span class="sxs-lookup"><span data-stu-id="e48f8-141">Example</span></span> 

##### <a name="request"></a><span data-ttu-id="e48f8-142">要求</span><span class="sxs-lookup"><span data-stu-id="e48f8-142">Request</span></span>

<span data-ttu-id="e48f8-143">次に、Delve からユーザーをオプトアウトして、組織全体のコンテンツの関連性に関する投稿を無効にする方法についての要求の例を示します。</span><span class="sxs-lookup"><span data-stu-id="e48f8-143">Here is an example request on how to opt-out a user from Delve and disable his contribution on content relevancy for the whole organization.</span></span>

```http
PATCH https://graph.microsoft.com/beta/me/settings
Content-type: application/json
Content-length: 37

{
  "contributionToContentDiscoveryDisabled": true
}
```

##### <a name="response"></a><span data-ttu-id="e48f8-144">応答</span><span class="sxs-lookup"><span data-stu-id="e48f8-144">Response</span></span>

<span data-ttu-id="e48f8-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e48f8-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```

#### <a name="batch-request"></a><span data-ttu-id="e48f8-148">バッチ要求</span><span class="sxs-lookup"><span data-stu-id="e48f8-148">Batch request</span></span>

<span data-ttu-id="e48f8-149">また、Delve から複数のユーザーをオプトアウトし、バッチ要求によって組織全体のコンテンツ関連性に対する貢献を無効にすることもできます。</span><span class="sxs-lookup"><span data-stu-id="e48f8-149">It's also possible to opt-out multiple users from Delve and disable their contribution on content relevancy for the whole organization through a batch request.</span></span>
<span data-ttu-id="e48f8-150">詳細については、「 [JSON のバッチ](/graph/json-batching)処理」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e48f8-150">To learn more, see [JSON batching](/graph/json-batching).</span></span>

<span data-ttu-id="e48f8-151">**重要**:[組織の管理](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US)役割グループのメンバーのみが複数のユーザーを更新できます。</span><span class="sxs-lookup"><span data-stu-id="e48f8-151">**Important**: Only members of the [Organization Management](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) role group can update multiple users.</span></span> 


