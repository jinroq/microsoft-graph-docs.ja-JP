---
title: サブスクリプションを一覧表示する
description: アプリ ID、ユーザー、およびテナントでのユーザーの役割に基づいて、Webhook サブスクリプションのプロパティとリレーションシップを取得します。
localization_priority: Priority
author: piotrci
ms.openlocfilehash: 603a918faa9153f4b8690613a2b9aed7b7f53420
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273144"
---
# <a name="list-subscriptions"></a><span data-ttu-id="5a4d8-103">サブスクリプションを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="5a4d8-103">List subscriptions</span></span>

<span data-ttu-id="5a4d8-104">アプリ ID、ユーザー、およびテナントでのユーザーの役割に基づいて、Webhook サブスクリプションのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-104">Retrieve the properties and relationships of webhook subscriptions, based on the app ID, the user, and the user's role with a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a4d8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5a4d8-105">Permissions</span></span>

<span data-ttu-id="5a4d8-106">この API は、次のアクセス許可スコープをサポートしています。アクセス許可の選択方法などに関する詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-106">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5a4d8-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5a4d8-107">Permission type</span></span>  | <span data-ttu-id="5a4d8-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5a4d8-108">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="5a4d8-109">[委任されたアクセス許可](/graph/auth-v2-user) (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5a4d8-109">[Delegated permission](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="5a4d8-110">[サブスクリプションの作成](subscription-post-subscriptions.md)に必要なロール、または Subscription.Read.All (後述)。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-110">Role required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="5a4d8-111">[委任されたアクセス許可](/graph/auth-v2-user) (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5a4d8-111">[Delegated permission](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="5a4d8-112">[サブスクリプションの作成](subscription-post-subscriptions.md)に必要なロール、または Subscription.Read.All (後述)。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-112">Role required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="5a4d8-113">アプリケーションのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="5a4d8-113">Application permission</span></span>](/graph/auth-v2-service) | <span data-ttu-id="5a4d8-114">[サブスクリプションの作成](subscription-post-subscriptions.md)に必要なロールです。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-114">Role required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="5a4d8-115">応答の結果は、呼び出し元アプリのコンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-115">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="5a4d8-116">次に、一般的なシナリオの概要を示します。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-116">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="5a4d8-117">基本シナリオ</span><span class="sxs-lookup"><span data-stu-id="5a4d8-117">Basic scenarios</span></span>

<span data-ttu-id="5a4d8-118">ほとんどの場合、アプリケーションは、現在サインインしているユーザーかディレクトリ (職場アカウントや学校アカウント) 内のすべてのユーザーに対してそのアプリケーションが元々作成していたサブスクリプションを取得しようとします。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-118">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="5a4d8-119">このようなシナリオでは、アプリがサブスクリプションを作成するために元々使用していたアクセス許可以外には、特別なアクセス許可は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-119">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="5a4d8-120">呼び出し元アプリのコンテキスト</span><span class="sxs-lookup"><span data-stu-id="5a4d8-120">Context of the calling app</span></span> | <span data-ttu-id="5a4d8-121">応答内容</span><span class="sxs-lookup"><span data-stu-id="5a4d8-121">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="5a4d8-122">サインイン ユーザーに代わってアプリが呼び出しを実行している (委任されたアクセス許可)。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-122">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="5a4d8-123">- および -</span><span class="sxs-lookup"><span data-stu-id="5a4d8-123">-and-</span></span><br/><span data-ttu-id="5a4d8-124">[サブスクリプションの作成](subscription-post-subscriptions.md)に必要な元のアクセス許可をアプリが持っている。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-124">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="5a4d8-125">注: これは、個人用の Microsoft アカウントと職場や学校のアカウントの両方に適用されます。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-125">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="5a4d8-126">**このアプリ**によって作成された、サインイン ユーザーのみのサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-126">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="5a4d8-127">アプリがそのアプリのために呼び出しを実行している (アプリケーションのアクセス許可)。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-127">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="5a4d8-128">- および -</span><span class="sxs-lookup"><span data-stu-id="5a4d8-128">-and-</span></span><br/><span data-ttu-id="5a4d8-129">[サブスクリプションの作成](subscription-post-subscriptions.md)に必要な元のアクセス許可をアプリが持っている。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-129">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="5a4d8-130">注: これは、職場や学校のアカウントにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-130">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="5a4d8-131">**このアプリ**によって作成された、アプリ自体またはディレクトリ内の任意のユーザーのサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-131">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="5a4d8-132">高度なシナリオ</span><span class="sxs-lookup"><span data-stu-id="5a4d8-132">Advanced scenarios</span></span>

<span data-ttu-id="5a4d8-133">場合によっては、アプリは、他のアプリによって作成されたサブスクリプションを取得しようとします。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-133">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="5a4d8-134">たとえば、ユーザーが、自分に代わって任意のアプリによって作成されたすべてのサブスクリプションを確認しようとすることがあります。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-134">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="5a4d8-135">また、管理者が、ディレクトリ内のすべてのアプリによって作成されたすべてのサブスクリプションを確認しようとすることがあります。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-135">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="5a4d8-136">このような場合、委任されたアクセス許可の Subscription.Read.All が必要になります。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-136">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="5a4d8-137">呼び出し元アプリのコンテキスト</span><span class="sxs-lookup"><span data-stu-id="5a4d8-137">Context of the calling app</span></span> | <span data-ttu-id="5a4d8-138">応答内容</span><span class="sxs-lookup"><span data-stu-id="5a4d8-138">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="5a4d8-139">サインイン ユーザーに代わってアプリが呼び出しを実行している (委任されたアクセス許可)。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-139">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="5a4d8-140">*ユーザーは管理者ではない*。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-140">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="5a4d8-141">- および -</span><span class="sxs-lookup"><span data-stu-id="5a4d8-141">-and-</span></span><br/><span data-ttu-id="5a4d8-142">Subscription.Read.All アクセス許可をアプリが持っている</span><span class="sxs-lookup"><span data-stu-id="5a4d8-142">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="5a4d8-143">注: これは、個人用の Microsoft アカウントと職場や学校のアカウントの両方に適用されます。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-143">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="5a4d8-144">**任意のアプリ**によって作成された、サインイン ユーザーのみのサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-144">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="5a4d8-145">サインイン ユーザーに代わってアプリが呼び出しを実行している (委任されたアクセス許可)。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-145">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="5a4d8-146">*ユーザーは管理者である*。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-146">*The user is an admin*.</span></span><br/><span data-ttu-id="5a4d8-147">- および -</span><span class="sxs-lookup"><span data-stu-id="5a4d8-147">-and-</span></span><br/><span data-ttu-id="5a4d8-148">Subscription.Read.All アクセス許可をアプリが持っている</span><span class="sxs-lookup"><span data-stu-id="5a4d8-148">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="5a4d8-149">注: これは、職場や学校のアカウントにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-149">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="5a4d8-150">**任意のアプリ**によって作成された、ディレクトリ内の**任意のユーザー**のサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-150">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a4d8-151">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5a4d8-151">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5a4d8-152">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5a4d8-152">Optional query parameters</span></span>

<span data-ttu-id="5a4d8-153">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-153">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5a4d8-154">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5a4d8-154">Request headers</span></span>

| <span data-ttu-id="5a4d8-155">名前</span><span class="sxs-lookup"><span data-stu-id="5a4d8-155">Name</span></span>       | <span data-ttu-id="5a4d8-156">型</span><span class="sxs-lookup"><span data-stu-id="5a4d8-156">Type</span></span> | <span data-ttu-id="5a4d8-157">説明</span><span class="sxs-lookup"><span data-stu-id="5a4d8-157">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5a4d8-158">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a4d8-158">Authorization</span></span>  | <span data-ttu-id="5a4d8-159">string</span><span class="sxs-lookup"><span data-stu-id="5a4d8-159">string</span></span>  | <span data-ttu-id="5a4d8-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a4d8-162">要求本文</span><span class="sxs-lookup"><span data-stu-id="5a4d8-162">Request body</span></span>

<span data-ttu-id="5a4d8-163">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-163">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a4d8-164">応答</span><span class="sxs-lookup"><span data-stu-id="5a4d8-164">Response</span></span>

<span data-ttu-id="5a4d8-165">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscription](../resources/subscription.md) オブジェクトの一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-165">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a4d8-166">例</span><span class="sxs-lookup"><span data-stu-id="5a4d8-166">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5a4d8-167">要求</span><span class="sxs-lookup"><span data-stu-id="5a4d8-167">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions
```

##### <a name="response"></a><span data-ttu-id="5a4d8-168">応答</span><span class="sxs-lookup"><span data-stu-id="5a4d8-168">Response</span></span>

<span data-ttu-id="5a4d8-169">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-169">Here's an an example of the response.</span></span>  <span data-ttu-id="5a4d8-170">簡潔にするために、切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-170">Note that it may be truncated for brevity.</span></span>  <span data-ttu-id="5a4d8-171">実際の呼び出しからは、サポートされているプロパティのうち、要求と呼び出し元のコンテキストに適しているものすべてが返されます。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-171">All supported properties appropriate for the request and the calling context will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 586

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions",
  "value": [
    {
      "id": "0fc0d6db-0073-42e5-a186-853da75fb308",
      "resource": "Users",
      "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
      "changeType": "updated,deleted",
      "clientState": null,
      "notificationUrl": "https://webhookappexample.azurewebsites.net/api/notifications",
      "expirationDateTime": "2018-03-12T05:00:00Z",
      "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5a4d8-172">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="5a4d8-172">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5a4d8-173">C#</span><span class="sxs-lookup"><span data-stu-id="5a4d8-173">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_subscriptions-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5a4d8-174">Javascript</span><span class="sxs-lookup"><span data-stu-id="5a4d8-174">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_subscriptions-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5a4d8-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a4d8-175">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_subscriptions-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/subscription-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/subscription-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/subscription-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

<span data-ttu-id="5a4d8-176">複数ページにわたるデータを要求が返す場合は、結果を管理しやすくするため、応答に `@odata.nextLink` プロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-176">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="5a4d8-177">詳細については、「[アプリで Microsoft Graph データをページングする](/graph/paging)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5a4d8-177">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
