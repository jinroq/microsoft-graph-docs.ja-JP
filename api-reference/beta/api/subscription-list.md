---
title: サブスクリプションを一覧表示する
description: " 詳細については、以下のシナリオを参照してください。"
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 3728c3fcf2fe3d78b243894632a363804a2f92c8
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638698"
---
# <a name="list-subscriptions"></a><span data-ttu-id="403dc-103">サブスクリプションを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="403dc-103">List subscriptions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="403dc-104">Webhook サブスクリプションの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="403dc-104">Retrieve a list of webhook subscriptions.</span></span> <span data-ttu-id="403dc-105">応答の内容は、アプリが呼び出しているコンテキストによって異なります。詳細については、以下のシナリオを参照してください。</span><span class="sxs-lookup"><span data-stu-id="403dc-105">The content of the response depends on the context in which the app is calling; see the scenarios below for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="403dc-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="403dc-106">Permissions</span></span>

<span data-ttu-id="403dc-107">この API は、次のアクセス許可スコープをサポートしています。アクセス許可の選択方法などに関する詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="403dc-107">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="403dc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="403dc-108">Permission type</span></span>  | <span data-ttu-id="403dc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="403dc-109">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="403dc-110">[委任](/graph/auth-v2-user)された(職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="403dc-110">[Delegated](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="403dc-111">サブスクリプションまたはサブスクリプションを[作成](subscription-post-subscriptions.md)するために必要なアクセス許可。 All (下を参照)。</span><span class="sxs-lookup"><span data-stu-id="403dc-111">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="403dc-112">[委任](/graph/auth-v2-user)された(個人 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="403dc-112">[Delegated](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="403dc-113">サブスクリプションまたはサブスクリプションを[作成](subscription-post-subscriptions.md)するために必要なアクセス許可。 All (下を参照)。</span><span class="sxs-lookup"><span data-stu-id="403dc-113">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="403dc-114">Application</span><span class="sxs-lookup"><span data-stu-id="403dc-114">Application</span></span>](/graph/auth-v2-service) | <span data-ttu-id="403dc-115">[サブスクリプションを作成](subscription-post-subscriptions.md)するために必要なアクセス許可。</span><span class="sxs-lookup"><span data-stu-id="403dc-115">Permission required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="403dc-116">応答の結果は、呼び出し元アプリのコンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="403dc-116">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="403dc-117">次に、一般的なシナリオの概要を示します。</span><span class="sxs-lookup"><span data-stu-id="403dc-117">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="403dc-118">基本シナリオ</span><span class="sxs-lookup"><span data-stu-id="403dc-118">Basic scenarios</span></span>

<span data-ttu-id="403dc-119">ほとんどの場合、アプリケーションは、現在サインインしているユーザーかディレクトリ (職場アカウントや学校アカウント) 内のすべてのユーザーに対してそのアプリケーションが元々作成していたサブスクリプションを取得しようとします。</span><span class="sxs-lookup"><span data-stu-id="403dc-119">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="403dc-120">このようなシナリオでは、アプリがサブスクリプションを作成するために元々使用していたアクセス許可以外には、特別なアクセス許可は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="403dc-120">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="403dc-121">呼び出し元アプリのコンテキスト</span><span class="sxs-lookup"><span data-stu-id="403dc-121">Context of the calling app</span></span> | <span data-ttu-id="403dc-122">応答内容</span><span class="sxs-lookup"><span data-stu-id="403dc-122">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="403dc-123">サインイン ユーザーに代わってアプリが呼び出しを実行している (委任されたアクセス許可)。</span><span class="sxs-lookup"><span data-stu-id="403dc-123">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="403dc-124">- および -</span><span class="sxs-lookup"><span data-stu-id="403dc-124">-and-</span></span><br/><span data-ttu-id="403dc-125">[サブスクリプションの作成](subscription-post-subscriptions.md)に必要な元のアクセス許可をアプリが持っている。</span><span class="sxs-lookup"><span data-stu-id="403dc-125">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="403dc-126">注: これは、個人用の Microsoft アカウントと職場や学校のアカウントの両方に適用されます。</span><span class="sxs-lookup"><span data-stu-id="403dc-126">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="403dc-127">**このアプリ**によって作成された、サインイン ユーザーのみのサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="403dc-127">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="403dc-128">アプリがそのアプリのために呼び出しを実行している (アプリケーションのアクセス許可)。</span><span class="sxs-lookup"><span data-stu-id="403dc-128">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="403dc-129">- および -</span><span class="sxs-lookup"><span data-stu-id="403dc-129">-and-</span></span><br/><span data-ttu-id="403dc-130">[サブスクリプションの作成](subscription-post-subscriptions.md)に必要な元のアクセス許可をアプリが持っている。</span><span class="sxs-lookup"><span data-stu-id="403dc-130">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="403dc-131">注: これは、職場や学校のアカウントにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="403dc-131">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="403dc-132">**このアプリ**によって作成された、アプリ自体またはディレクトリ内の任意のユーザーのサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="403dc-132">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="403dc-133">高度なシナリオ</span><span class="sxs-lookup"><span data-stu-id="403dc-133">Advanced scenarios</span></span>

<span data-ttu-id="403dc-134">場合によっては、アプリは、他のアプリによって作成されたサブスクリプションを取得しようとします。</span><span class="sxs-lookup"><span data-stu-id="403dc-134">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="403dc-135">たとえば、ユーザーが、自分に代わって任意のアプリによって作成されたすべてのサブスクリプションを確認しようとすることがあります。</span><span class="sxs-lookup"><span data-stu-id="403dc-135">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="403dc-136">また、管理者が、ディレクトリ内のすべてのアプリによって作成されたすべてのサブスクリプションを確認しようとすることがあります。</span><span class="sxs-lookup"><span data-stu-id="403dc-136">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="403dc-137">このような場合、委任されたアクセス許可の Subscription.Read.All が必要になります。</span><span class="sxs-lookup"><span data-stu-id="403dc-137">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="403dc-138">呼び出し元アプリのコンテキスト</span><span class="sxs-lookup"><span data-stu-id="403dc-138">Context of the calling app</span></span> | <span data-ttu-id="403dc-139">応答内容</span><span class="sxs-lookup"><span data-stu-id="403dc-139">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="403dc-140">サインイン ユーザーに代わってアプリが呼び出しを実行している (委任されたアクセス許可)。</span><span class="sxs-lookup"><span data-stu-id="403dc-140">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="403dc-141">*ユーザーは管理者ではない*。</span><span class="sxs-lookup"><span data-stu-id="403dc-141">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="403dc-142">- および -</span><span class="sxs-lookup"><span data-stu-id="403dc-142">-and-</span></span><br/><span data-ttu-id="403dc-143">Subscription.Read.All アクセス許可をアプリが持っている</span><span class="sxs-lookup"><span data-stu-id="403dc-143">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="403dc-144">注: これは、個人用の Microsoft アカウントと職場や学校のアカウントの両方に適用されます。</span><span class="sxs-lookup"><span data-stu-id="403dc-144">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="403dc-145">**任意のアプリ**によって作成された、サインイン ユーザーのみのサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="403dc-145">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="403dc-146">サインイン ユーザーに代わってアプリが呼び出しを実行している (委任されたアクセス許可)。</span><span class="sxs-lookup"><span data-stu-id="403dc-146">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="403dc-147">*ユーザーは管理者である*。</span><span class="sxs-lookup"><span data-stu-id="403dc-147">*The user is an admin*.</span></span><br/><span data-ttu-id="403dc-148">- および -</span><span class="sxs-lookup"><span data-stu-id="403dc-148">-and-</span></span><br/><span data-ttu-id="403dc-149">Subscription.Read.All アクセス許可をアプリが持っている</span><span class="sxs-lookup"><span data-stu-id="403dc-149">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="403dc-150">注: これは、職場や学校のアカウントにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="403dc-150">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="403dc-151">**任意のアプリ**によって作成された、ディレクトリ内の**任意のユーザー**のサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="403dc-151">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="403dc-152">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="403dc-152">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="403dc-153">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="403dc-153">Optional query parameters</span></span>

<span data-ttu-id="403dc-154">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="403dc-154">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="403dc-155">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="403dc-155">Request headers</span></span>

| <span data-ttu-id="403dc-156">名前</span><span class="sxs-lookup"><span data-stu-id="403dc-156">Name</span></span>       | <span data-ttu-id="403dc-157">型</span><span class="sxs-lookup"><span data-stu-id="403dc-157">Type</span></span> | <span data-ttu-id="403dc-158">説明</span><span class="sxs-lookup"><span data-stu-id="403dc-158">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="403dc-159">Authorization</span><span class="sxs-lookup"><span data-stu-id="403dc-159">Authorization</span></span>  | <span data-ttu-id="403dc-160">string</span><span class="sxs-lookup"><span data-stu-id="403dc-160">string</span></span>  | <span data-ttu-id="403dc-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="403dc-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="403dc-163">要求本文</span><span class="sxs-lookup"><span data-stu-id="403dc-163">Request body</span></span>

<span data-ttu-id="403dc-164">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="403dc-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="403dc-165">応答</span><span class="sxs-lookup"><span data-stu-id="403dc-165">Response</span></span>

<span data-ttu-id="403dc-166">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscription](../resources/subscription.md) オブジェクトの一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="403dc-166">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="403dc-167">例</span><span class="sxs-lookup"><span data-stu-id="403dc-167">Example</span></span>

##### <a name="request"></a><span data-ttu-id="403dc-168">要求</span><span class="sxs-lookup"><span data-stu-id="403dc-168">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions
```

##### <a name="response"></a><span data-ttu-id="403dc-169">応答</span><span class="sxs-lookup"><span data-stu-id="403dc-169">Response</span></span>

<span data-ttu-id="403dc-170">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="403dc-170">Here is an example of the response.</span></span> <span data-ttu-id="403dc-171">注: 簡潔にするために、ここに示す応答は切り捨てられる場合があります。</span><span class="sxs-lookup"><span data-stu-id="403dc-171">Note: The response shown here may be truncated for brevity.</span></span> <span data-ttu-id="403dc-172">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="403dc-172">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 586

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="403dc-173">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="403dc-173">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="403dc-174">Visual</span><span class="sxs-lookup"><span data-stu-id="403dc-174">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_subscriptions-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="403dc-175">Java</span><span class="sxs-lookup"><span data-stu-id="403dc-175">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_subscriptions-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/subscription-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->

<span data-ttu-id="403dc-176">複数ページにわたるデータを要求が返す場合は、結果を管理しやすくするため、応答に `@odata.nextLink` プロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="403dc-176">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="403dc-177">詳細については、「[アプリで Microsoft Graph データをページングする](/graph/paging)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="403dc-177">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
