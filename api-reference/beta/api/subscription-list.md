---
title: リストの購読
description: " 詳細については以下のシナリオを参照してください。"
ms.openlocfilehash: ad5e97a9b721a9e557e01dd4743b53a52c6dc8d7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073409"
---
# <a name="list-subscriptions"></a><span data-ttu-id="f5faf-103">リストの購読</span><span class="sxs-lookup"><span data-stu-id="f5faf-103">List subscriptions</span></span>

> <span data-ttu-id="f5faf-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f5faf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5faf-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5faf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f5faf-106">Webhook サブスクリプションの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="f5faf-106">Retrieve a list of webhook subscriptions.</span></span> <span data-ttu-id="f5faf-107">応答の内容では、アプリケーションを呼び出す; コンテキストによって異なります。詳細については以下のシナリオを参照してください。</span><span class="sxs-lookup"><span data-stu-id="f5faf-107">The content of the response depends on the context in which the app is calling; see the scenarios below for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5faf-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="f5faf-108">Permissions</span></span>

<span data-ttu-id="f5faf-109">この API には、次のアクセス許可のスコープがサポートされています。アクセス許可] を選択する方法などの詳細については、[アクセス許可](/graph/permissions-reference)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f5faf-109">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f5faf-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f5faf-110">Permission type</span></span>  | <span data-ttu-id="f5faf-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f5faf-111">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="f5faf-112">[委任](/graph/auth-v2-user)(職場、学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f5faf-112">[Delegated](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="f5faf-113">[サブスクリプションを作成](subscription-post-subscriptions.md)または Subscription.Read.All (下記参照) に必要なアクセスを許可します。</span><span class="sxs-lookup"><span data-stu-id="f5faf-113">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="f5faf-114">[委任](/graph/auth-v2-user)(個人用の Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f5faf-114">[Delegated](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="f5faf-115">[サブスクリプションを作成](subscription-post-subscriptions.md)または Subscription.Read.All (下記参照) に必要なアクセスを許可します。</span><span class="sxs-lookup"><span data-stu-id="f5faf-115">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="f5faf-116">Application</span><span class="sxs-lookup"><span data-stu-id="f5faf-116">Application</span></span>](/graph/auth-v2-service) | <span data-ttu-id="f5faf-117">[サブスクリプションを作成](subscription-post-subscriptions.md)するために必要なアクセスを許可します。</span><span class="sxs-lookup"><span data-stu-id="f5faf-117">Permission required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="f5faf-118">応答の結果は、呼び出し元のアプリケーションのコンテキストに基づいています。</span><span class="sxs-lookup"><span data-stu-id="f5faf-118">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="f5faf-119">以下は、一般的なシナリオの概要です。</span><span class="sxs-lookup"><span data-stu-id="f5faf-119">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="f5faf-120">基本的なシナリオ</span><span class="sxs-lookup"><span data-stu-id="f5faf-120">Basic scenarios</span></span>

<span data-ttu-id="f5faf-121">ほとんどの場合、アプリケーションは、最初に作成された、現在サインインしているユーザーやディレクトリ (仕事/学校のアカウント) のすべてのユーザーのサブスクリプションを取得しようとします。</span><span class="sxs-lookup"><span data-stu-id="f5faf-121">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="f5faf-122">これらのシナリオは不要のもの以外の特殊なアクセス許可のサブスクリプションを作成する最初に使用するアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="f5faf-122">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="f5faf-123">呼び出し元のアプリケーションのコンテキスト</span><span class="sxs-lookup"><span data-stu-id="f5faf-123">Context of the calling app</span></span> | <span data-ttu-id="f5faf-124">応答が含まれています</span><span class="sxs-lookup"><span data-stu-id="f5faf-124">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="f5faf-125">サインインしているユーザー (委任されたアクセス許可) のため、アプリケーションを呼び出しています。</span><span class="sxs-lookup"><span data-stu-id="f5faf-125">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="f5faf-126">- と -</span><span class="sxs-lookup"><span data-stu-id="f5faf-126">-and-</span></span><br/><span data-ttu-id="f5faf-127">アプリケーションでは、[サブスクリプションを作成](subscription-post-subscriptions.md)するために必要な元の権限を持っています。</span><span class="sxs-lookup"><span data-stu-id="f5faf-127">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="f5faf-128">注意: 個人用の Microsoft アカウントとアカウントの仕事/学校の両方に適用します。</span><span class="sxs-lookup"><span data-stu-id="f5faf-128">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="f5faf-129">サブスクリプションは、サインインしているユーザーに対してのみ、**このアプリケーション**によって作成されました。</span><span class="sxs-lookup"><span data-stu-id="f5faf-129">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="f5faf-130">自体 (アプリケーションのアクセス許可) のため、アプリケーションを呼び出しています。</span><span class="sxs-lookup"><span data-stu-id="f5faf-130">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="f5faf-131">- と -</span><span class="sxs-lookup"><span data-stu-id="f5faf-131">-and-</span></span><br/><span data-ttu-id="f5faf-132">アプリケーションでは、[サブスクリプションを作成](subscription-post-subscriptions.md)するために必要な元の権限を持っています。</span><span class="sxs-lookup"><span data-stu-id="f5faf-132">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="f5faf-133">注意: 仕事/学校のアカウントのみに適用します。</span><span class="sxs-lookup"><span data-stu-id="f5faf-133">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="f5faf-134">自体やディレクトリ内のすべてのユーザーに、**このアプリケーション**によって作成されたサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="f5faf-134">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="f5faf-135">高度なシナリオ</span><span class="sxs-lookup"><span data-stu-id="f5faf-135">Advanced scenarios</span></span>

<span data-ttu-id="f5faf-136">場合によっては、アプリケーションは、他のアプリケーションによって作成されたサブスクリプションを取得しようとします。</span><span class="sxs-lookup"><span data-stu-id="f5faf-136">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="f5faf-137">たとえば、ユーザーは代わりに他のアプリケーションによって作成されたすべてのサブスクリプションを参照してください希望しています。</span><span class="sxs-lookup"><span data-stu-id="f5faf-137">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="f5faf-138">または、管理者はそのディレクトリ内のすべてのアプリケーションからのすべてのサブスクリプションを参照してくださいすることがあります。</span><span class="sxs-lookup"><span data-stu-id="f5faf-138">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="f5faf-139">このような状況では、Subscription.Read.All の委任されたアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="f5faf-139">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="f5faf-140">呼び出し元のアプリケーションのコンテキスト</span><span class="sxs-lookup"><span data-stu-id="f5faf-140">Context of the calling app</span></span> | <span data-ttu-id="f5faf-141">応答が含まれています</span><span class="sxs-lookup"><span data-stu-id="f5faf-141">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="f5faf-142">サインインしているユーザー (委任されたアクセス許可) のため、アプリケーションを呼び出しています。</span><span class="sxs-lookup"><span data-stu-id="f5faf-142">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="f5faf-143">*ユーザーは管理者以外*は。</span><span class="sxs-lookup"><span data-stu-id="f5faf-143">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="f5faf-144">- と -</span><span class="sxs-lookup"><span data-stu-id="f5faf-144">-and-</span></span><br/><span data-ttu-id="f5faf-145">アプリには、アクセス許可が Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5faf-145">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="f5faf-146">注意: 個人用の Microsoft アカウントとアカウントの仕事/学校の両方に適用します。</span><span class="sxs-lookup"><span data-stu-id="f5faf-146">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="f5faf-147">サブスクリプションは、サインインしているユーザーに対してのみ **、アプリケーション**によって作成されました。</span><span class="sxs-lookup"><span data-stu-id="f5faf-147">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="f5faf-148">サインインしているユーザー (委任されたアクセス許可) のため、アプリケーションを呼び出しています。</span><span class="sxs-lookup"><span data-stu-id="f5faf-148">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="f5faf-149">*ユーザーは管理者*です。</span><span class="sxs-lookup"><span data-stu-id="f5faf-149">*The user is an admin*.</span></span><br/><span data-ttu-id="f5faf-150">- と -</span><span class="sxs-lookup"><span data-stu-id="f5faf-150">-and-</span></span><br/><span data-ttu-id="f5faf-151">アプリには、アクセス許可が Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5faf-151">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="f5faf-152">注意: 仕事/学校のアカウントのみに適用します。</span><span class="sxs-lookup"><span data-stu-id="f5faf-152">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="f5faf-153">ディレクトリ内の**すべてのユーザー**の**すべてのアプリケーション**によって作成されるサブスクリプションです。</span><span class="sxs-lookup"><span data-stu-id="f5faf-153">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5faf-154">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f5faf-154">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f5faf-155">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f5faf-155">Optional query parameters</span></span>

<span data-ttu-id="f5faf-156">このメソッドは、応答をカスタマイズするために[OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="f5faf-156">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f5faf-157">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f5faf-157">Request headers</span></span>

| <span data-ttu-id="f5faf-158">名前</span><span class="sxs-lookup"><span data-stu-id="f5faf-158">Name</span></span>       | <span data-ttu-id="f5faf-159">型</span><span class="sxs-lookup"><span data-stu-id="f5faf-159">Type</span></span> | <span data-ttu-id="f5faf-160">説明</span><span class="sxs-lookup"><span data-stu-id="f5faf-160">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f5faf-161">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5faf-161">Authorization</span></span>  | <span data-ttu-id="f5faf-162">string</span><span class="sxs-lookup"><span data-stu-id="f5faf-162">string</span></span>  | <span data-ttu-id="f5faf-p108">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f5faf-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5faf-165">要求本文</span><span class="sxs-lookup"><span data-stu-id="f5faf-165">Request body</span></span>

<span data-ttu-id="f5faf-166">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f5faf-166">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5faf-167">応答</span><span class="sxs-lookup"><span data-stu-id="f5faf-167">Response</span></span>

<span data-ttu-id="f5faf-168">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文のオブジェクトの[サブスクリプション](../resources/subscription.md)の一覧です。</span><span class="sxs-lookup"><span data-stu-id="f5faf-168">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5faf-169">例</span><span class="sxs-lookup"><span data-stu-id="f5faf-169">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f5faf-170">要求</span><span class="sxs-lookup"><span data-stu-id="f5faf-170">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions
```

##### <a name="response"></a><span data-ttu-id="f5faf-171">応答</span><span class="sxs-lookup"><span data-stu-id="f5faf-171">Response</span></span>

<span data-ttu-id="f5faf-172">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="f5faf-172">Here is an example of the response.</span></span> <span data-ttu-id="f5faf-173">注: ここに示す応答は簡潔にするためにあります。</span><span class="sxs-lookup"><span data-stu-id="f5faf-173">Note: The response shown here may be truncated for brevity.</span></span> <span data-ttu-id="f5faf-174">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f5faf-174">All of the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

<span data-ttu-id="f5faf-175">応答が含まれて、要求にデータの複数のページが返されるとき、 `@odata.nextLink` 、結果を管理するためのプロパティです。</span><span class="sxs-lookup"><span data-stu-id="f5faf-175">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="f5faf-176">詳細については、[アプリケーションでは、Microsoft Graph のページング データ](/graph/paging)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f5faf-176">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
