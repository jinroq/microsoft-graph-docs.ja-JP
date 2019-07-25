---
title: サブスクリプションを一覧表示する
description: " 詳細については、以下のシナリオを参照してください。"
localization_priority: Normal
author: piotrci
ms.openlocfilehash: b42b84c56638c206b3ea440efba880e4ab024601
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869456"
---
# <a name="list-subscriptions"></a><span data-ttu-id="c3e78-103">サブスクリプションを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c3e78-103">List subscriptions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3e78-104">Webhook サブスクリプションの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="c3e78-104">Retrieve a list of webhook subscriptions.</span></span> <span data-ttu-id="c3e78-105">応答の内容は、アプリが呼び出しているコンテキストによって異なります。詳細については、以下のシナリオを参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3e78-105">The content of the response depends on the context in which the app is calling; see the scenarios below for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3e78-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c3e78-106">Permissions</span></span>

<span data-ttu-id="c3e78-107">この API は、次のアクセス許可スコープをサポートしています。アクセス許可の選択方法などに関する詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3e78-107">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c3e78-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c3e78-108">Permission type</span></span>  | <span data-ttu-id="c3e78-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c3e78-109">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="c3e78-110">[委任](/graph/auth-v2-user)された(職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c3e78-110">[Delegated](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="c3e78-111">サブスクリプションまたはサブスクリプションを[作成](subscription-post-subscriptions.md)するために必要なアクセス許可。 All (下を参照)。</span><span class="sxs-lookup"><span data-stu-id="c3e78-111">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="c3e78-112">[委任](/graph/auth-v2-user)された(個人 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c3e78-112">[Delegated](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="c3e78-113">サブスクリプションまたはサブスクリプションを[作成](subscription-post-subscriptions.md)するために必要なアクセス許可。 All (下を参照)。</span><span class="sxs-lookup"><span data-stu-id="c3e78-113">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="c3e78-114">Application</span><span class="sxs-lookup"><span data-stu-id="c3e78-114">Application</span></span>](/graph/auth-v2-service) | <span data-ttu-id="c3e78-115">[サブスクリプションを作成](subscription-post-subscriptions.md)するために必要なアクセス許可。</span><span class="sxs-lookup"><span data-stu-id="c3e78-115">Permission required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="c3e78-116">応答の結果は、呼び出し元アプリのコンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="c3e78-116">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="c3e78-117">次に、一般的なシナリオの概要を示します。</span><span class="sxs-lookup"><span data-stu-id="c3e78-117">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="c3e78-118">基本シナリオ</span><span class="sxs-lookup"><span data-stu-id="c3e78-118">Basic scenarios</span></span>

<span data-ttu-id="c3e78-119">ほとんどの場合、アプリケーションは、現在サインインしているユーザーかディレクトリ (職場アカウントや学校アカウント) 内のすべてのユーザーに対してそのアプリケーションが元々作成していたサブスクリプションを取得しようとします。</span><span class="sxs-lookup"><span data-stu-id="c3e78-119">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="c3e78-120">このようなシナリオでは、アプリがサブスクリプションを作成するために元々使用していたアクセス許可以外には、特別なアクセス許可は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="c3e78-120">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="c3e78-121">呼び出し元アプリのコンテキスト</span><span class="sxs-lookup"><span data-stu-id="c3e78-121">Context of the calling app</span></span> | <span data-ttu-id="c3e78-122">応答内容</span><span class="sxs-lookup"><span data-stu-id="c3e78-122">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="c3e78-123">サインイン ユーザーに代わってアプリが呼び出しを実行している (委任されたアクセス許可)。</span><span class="sxs-lookup"><span data-stu-id="c3e78-123">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="c3e78-124">- および -</span><span class="sxs-lookup"><span data-stu-id="c3e78-124">-and-</span></span><br/><span data-ttu-id="c3e78-125">[サブスクリプションの作成](subscription-post-subscriptions.md)に必要な元のアクセス許可をアプリが持っている。</span><span class="sxs-lookup"><span data-stu-id="c3e78-125">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="c3e78-126">注: これは、個人用の Microsoft アカウントと職場や学校のアカウントの両方に適用されます。</span><span class="sxs-lookup"><span data-stu-id="c3e78-126">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="c3e78-127">**このアプリ**によって作成された、サインイン ユーザーのみのサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="c3e78-127">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="c3e78-128">アプリがそのアプリのために呼び出しを実行している (アプリケーションのアクセス許可)。</span><span class="sxs-lookup"><span data-stu-id="c3e78-128">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="c3e78-129">- および -</span><span class="sxs-lookup"><span data-stu-id="c3e78-129">-and-</span></span><br/><span data-ttu-id="c3e78-130">[サブスクリプションの作成](subscription-post-subscriptions.md)に必要な元のアクセス許可をアプリが持っている。</span><span class="sxs-lookup"><span data-stu-id="c3e78-130">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="c3e78-131">注: これは、職場や学校のアカウントにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="c3e78-131">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="c3e78-132">**このアプリ**によって作成された、アプリ自体またはディレクトリ内の任意のユーザーのサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="c3e78-132">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="c3e78-133">高度なシナリオ</span><span class="sxs-lookup"><span data-stu-id="c3e78-133">Advanced scenarios</span></span>

<span data-ttu-id="c3e78-134">場合によっては、アプリは、他のアプリによって作成されたサブスクリプションを取得しようとします。</span><span class="sxs-lookup"><span data-stu-id="c3e78-134">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="c3e78-135">たとえば、ユーザーが、自分に代わって任意のアプリによって作成されたすべてのサブスクリプションを確認しようとすることがあります。</span><span class="sxs-lookup"><span data-stu-id="c3e78-135">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="c3e78-136">また、管理者が、ディレクトリ内のすべてのアプリによって作成されたすべてのサブスクリプションを確認しようとすることがあります。</span><span class="sxs-lookup"><span data-stu-id="c3e78-136">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="c3e78-137">このような場合、委任されたアクセス許可の Subscription.Read.All が必要になります。</span><span class="sxs-lookup"><span data-stu-id="c3e78-137">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="c3e78-138">呼び出し元アプリのコンテキスト</span><span class="sxs-lookup"><span data-stu-id="c3e78-138">Context of the calling app</span></span> | <span data-ttu-id="c3e78-139">応答内容</span><span class="sxs-lookup"><span data-stu-id="c3e78-139">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="c3e78-140">サインイン ユーザーに代わってアプリが呼び出しを実行している (委任されたアクセス許可)。</span><span class="sxs-lookup"><span data-stu-id="c3e78-140">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="c3e78-141">*ユーザーは管理者ではない*。</span><span class="sxs-lookup"><span data-stu-id="c3e78-141">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="c3e78-142">- および -</span><span class="sxs-lookup"><span data-stu-id="c3e78-142">-and-</span></span><br/><span data-ttu-id="c3e78-143">Subscription.Read.All アクセス許可をアプリが持っている</span><span class="sxs-lookup"><span data-stu-id="c3e78-143">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="c3e78-144">注: これは、個人用の Microsoft アカウントと職場や学校のアカウントの両方に適用されます。</span><span class="sxs-lookup"><span data-stu-id="c3e78-144">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="c3e78-145">**任意のアプリ**によって作成された、サインイン ユーザーのみのサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="c3e78-145">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="c3e78-146">サインイン ユーザーに代わってアプリが呼び出しを実行している (委任されたアクセス許可)。</span><span class="sxs-lookup"><span data-stu-id="c3e78-146">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="c3e78-147">*ユーザーは管理者である*。</span><span class="sxs-lookup"><span data-stu-id="c3e78-147">*The user is an admin*.</span></span><br/><span data-ttu-id="c3e78-148">- および -</span><span class="sxs-lookup"><span data-stu-id="c3e78-148">-and-</span></span><br/><span data-ttu-id="c3e78-149">Subscription.Read.All アクセス許可をアプリが持っている</span><span class="sxs-lookup"><span data-stu-id="c3e78-149">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="c3e78-150">注: これは、職場や学校のアカウントにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="c3e78-150">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="c3e78-151">**任意のアプリ**によって作成された、ディレクトリ内の**任意のユーザー**のサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="c3e78-151">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3e78-152">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c3e78-152">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c3e78-153">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c3e78-153">Optional query parameters</span></span>

<span data-ttu-id="c3e78-154">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="c3e78-154">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3e78-155">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3e78-155">Request headers</span></span>

| <span data-ttu-id="c3e78-156">名前</span><span class="sxs-lookup"><span data-stu-id="c3e78-156">Name</span></span>       | <span data-ttu-id="c3e78-157">型</span><span class="sxs-lookup"><span data-stu-id="c3e78-157">Type</span></span> | <span data-ttu-id="c3e78-158">説明</span><span class="sxs-lookup"><span data-stu-id="c3e78-158">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c3e78-159">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3e78-159">Authorization</span></span>  | <span data-ttu-id="c3e78-160">string</span><span class="sxs-lookup"><span data-stu-id="c3e78-160">string</span></span>  | <span data-ttu-id="c3e78-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c3e78-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3e78-163">要求本文</span><span class="sxs-lookup"><span data-stu-id="c3e78-163">Request body</span></span>

<span data-ttu-id="c3e78-164">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c3e78-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3e78-165">応答</span><span class="sxs-lookup"><span data-stu-id="c3e78-165">Response</span></span>

<span data-ttu-id="c3e78-166">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscription](../resources/subscription.md) オブジェクトの一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="c3e78-166">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3e78-167">例</span><span class="sxs-lookup"><span data-stu-id="c3e78-167">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c3e78-168">要求</span><span class="sxs-lookup"><span data-stu-id="c3e78-168">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c3e78-169">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c3e78-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c3e78-170">C#</span><span class="sxs-lookup"><span data-stu-id="c3e78-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c3e78-171">Javascript</span><span class="sxs-lookup"><span data-stu-id="c3e78-171">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c3e78-172">目的-C</span><span class="sxs-lookup"><span data-stu-id="c3e78-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c3e78-173">Java</span><span class="sxs-lookup"><span data-stu-id="c3e78-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c3e78-174">応答</span><span class="sxs-lookup"><span data-stu-id="c3e78-174">Response</span></span>

<span data-ttu-id="c3e78-175">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c3e78-175">Here is an example of the response.</span></span> <span data-ttu-id="c3e78-176">注: 簡潔にするために、ここに示す応答は切り捨てられる場合があります。</span><span class="sxs-lookup"><span data-stu-id="c3e78-176">Note: The response shown here may be truncated for brevity.</span></span> <span data-ttu-id="c3e78-177">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c3e78-177">All of the properties will be returned from an actual call.</span></span>

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
  ]
}
-->

<span data-ttu-id="c3e78-178">複数ページにわたるデータを要求が返す場合は、結果を管理しやすくするため、応答に `@odata.nextLink` プロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="c3e78-178">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="c3e78-179">詳細については、「[アプリで Microsoft Graph データをページングする](/graph/paging)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3e78-179">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
