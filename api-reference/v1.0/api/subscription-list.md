---
title: リストの購読
description: プロパティとアプリケーション ID、ユーザー、およびテナントのユーザーのロールに基づいて、webhook サブスクリプションの関係を取得します。
ms.openlocfilehash: df52fd51de120002a7eff57b32715b281744be93
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023807"
---
# <a name="list-subscriptions"></a><span data-ttu-id="dae6c-103">リストの購読</span><span class="sxs-lookup"><span data-stu-id="dae6c-103">List subscriptions</span></span>

<span data-ttu-id="dae6c-104">プロパティとアプリケーション ID、ユーザー、およびテナントのユーザーのロールに基づいて、webhook サブスクリプションの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="dae6c-104">Retrieve the properties and relationships of webhook subscriptions, based on the app ID, the user, and the user's role with a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="dae6c-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="dae6c-105">Permissions</span></span>

<span data-ttu-id="dae6c-106">この API には、次のアクセス許可のスコープがサポートされています。アクセス許可] を選択する方法などの詳細については、[アクセス許可](/graph/permissions-reference)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dae6c-106">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dae6c-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dae6c-107">Permission type</span></span>  | <span data-ttu-id="dae6c-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dae6c-108">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="dae6c-109">[委任されたアクセス許可](/graph/auth-v2-user)(職場、学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dae6c-109">[Delegated permission](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="dae6c-110">[サブスクリプションを作成](subscription-post-subscriptions.md)または Subscription.Read.All (下記参照) に必要なロールです。</span><span class="sxs-lookup"><span data-stu-id="dae6c-110">Role required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="dae6c-111">[委任されたアクセス許可](/graph/auth-v2-user)(個人用の Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dae6c-111">[Delegated permission](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="dae6c-112">[サブスクリプションを作成](subscription-post-subscriptions.md)または Subscription.Read.All (下記参照) に必要なロールです。</span><span class="sxs-lookup"><span data-stu-id="dae6c-112">Role required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="dae6c-113">アプリケーションのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="dae6c-113">Application permission</span></span>](/graph/auth-v2-service) | <span data-ttu-id="dae6c-114">[サブスクリプションを作成](subscription-post-subscriptions.md)するために必要なロールです。</span><span class="sxs-lookup"><span data-stu-id="dae6c-114">Role required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="dae6c-115">応答の結果は、呼び出し元のアプリケーションのコンテキストに基づいています。</span><span class="sxs-lookup"><span data-stu-id="dae6c-115">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="dae6c-116">以下は、一般的なシナリオの概要です。</span><span class="sxs-lookup"><span data-stu-id="dae6c-116">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="dae6c-117">基本的なシナリオ</span><span class="sxs-lookup"><span data-stu-id="dae6c-117">Basic scenarios</span></span>

<span data-ttu-id="dae6c-118">ほとんどの場合、アプリケーションは、最初に作成された、現在サインインしているユーザーやディレクトリ (仕事/学校のアカウント) のすべてのユーザーのサブスクリプションを取得しようとします。</span><span class="sxs-lookup"><span data-stu-id="dae6c-118">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="dae6c-119">これらのシナリオは不要のもの以外の特殊なアクセス許可のサブスクリプションを作成する最初に使用するアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="dae6c-119">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="dae6c-120">呼び出し元のアプリケーションのコンテキスト</span><span class="sxs-lookup"><span data-stu-id="dae6c-120">Context of the calling app</span></span> | <span data-ttu-id="dae6c-121">応答が含まれています</span><span class="sxs-lookup"><span data-stu-id="dae6c-121">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="dae6c-122">サインインしているユーザー (委任されたアクセス許可) のため、アプリケーションを呼び出しています。</span><span class="sxs-lookup"><span data-stu-id="dae6c-122">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="dae6c-123">- と -</span><span class="sxs-lookup"><span data-stu-id="dae6c-123">-and-</span></span><br/><span data-ttu-id="dae6c-124">アプリケーションでは、[サブスクリプションを作成](subscription-post-subscriptions.md)するために必要な元の権限を持っています。</span><span class="sxs-lookup"><span data-stu-id="dae6c-124">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="dae6c-125">注意: 個人用の Microsoft アカウントとアカウントの仕事/学校の両方に適用します。</span><span class="sxs-lookup"><span data-stu-id="dae6c-125">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="dae6c-126">サブスクリプションは、サインインしているユーザーに対してのみ、**このアプリケーション**によって作成されました。</span><span class="sxs-lookup"><span data-stu-id="dae6c-126">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="dae6c-127">自体 (アプリケーションのアクセス許可) のため、アプリケーションを呼び出しています。</span><span class="sxs-lookup"><span data-stu-id="dae6c-127">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="dae6c-128">- と -</span><span class="sxs-lookup"><span data-stu-id="dae6c-128">-and-</span></span><br/><span data-ttu-id="dae6c-129">アプリケーションでは、[サブスクリプションを作成](subscription-post-subscriptions.md)するために必要な元の権限を持っています。</span><span class="sxs-lookup"><span data-stu-id="dae6c-129">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="dae6c-130">注意: 仕事/学校のアカウントのみに適用します。</span><span class="sxs-lookup"><span data-stu-id="dae6c-130">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="dae6c-131">自体やディレクトリ内のすべてのユーザーに、**このアプリケーション**によって作成されたサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="dae6c-131">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="dae6c-132">高度なシナリオ</span><span class="sxs-lookup"><span data-stu-id="dae6c-132">Advanced scenarios</span></span>

<span data-ttu-id="dae6c-133">場合によっては、アプリケーションは、他のアプリケーションによって作成されたサブスクリプションを取得しようとします。</span><span class="sxs-lookup"><span data-stu-id="dae6c-133">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="dae6c-134">たとえば、ユーザーは代わりに他のアプリケーションによって作成されたすべてのサブスクリプションを参照してください希望しています。</span><span class="sxs-lookup"><span data-stu-id="dae6c-134">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="dae6c-135">または、管理者はそのディレクトリ内のすべてのアプリケーションからのすべてのサブスクリプションを参照してくださいすることがあります。</span><span class="sxs-lookup"><span data-stu-id="dae6c-135">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="dae6c-136">このような状況では、Subscription.Read.All の委任されたアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="dae6c-136">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="dae6c-137">呼び出し元のアプリケーションのコンテキスト</span><span class="sxs-lookup"><span data-stu-id="dae6c-137">Context of the calling app</span></span> | <span data-ttu-id="dae6c-138">応答が含まれています</span><span class="sxs-lookup"><span data-stu-id="dae6c-138">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="dae6c-139">サインインしているユーザー (委任されたアクセス許可) のため、アプリケーションを呼び出しています。</span><span class="sxs-lookup"><span data-stu-id="dae6c-139">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="dae6c-140">*ユーザーは管理者以外*は。</span><span class="sxs-lookup"><span data-stu-id="dae6c-140">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="dae6c-141">- と -</span><span class="sxs-lookup"><span data-stu-id="dae6c-141">-and-</span></span><br/><span data-ttu-id="dae6c-142">アプリには、アクセス許可が Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="dae6c-142">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="dae6c-143">注意: 個人用の Microsoft アカウントとアカウントの仕事/学校の両方に適用します。</span><span class="sxs-lookup"><span data-stu-id="dae6c-143">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="dae6c-144">サブスクリプションは、サインインしているユーザーに対してのみ **、アプリケーション**によって作成されました。</span><span class="sxs-lookup"><span data-stu-id="dae6c-144">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="dae6c-145">サインインしているユーザー (委任されたアクセス許可) のため、アプリケーションを呼び出しています。</span><span class="sxs-lookup"><span data-stu-id="dae6c-145">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="dae6c-146">*ユーザーは管理者*です。</span><span class="sxs-lookup"><span data-stu-id="dae6c-146">*The user is an admin*.</span></span><br/><span data-ttu-id="dae6c-147">- と -</span><span class="sxs-lookup"><span data-stu-id="dae6c-147">-and-</span></span><br/><span data-ttu-id="dae6c-148">アプリには、アクセス許可が Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="dae6c-148">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="dae6c-149">注意: 仕事/学校のアカウントのみに適用します。</span><span class="sxs-lookup"><span data-stu-id="dae6c-149">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="dae6c-150">ディレクトリ内の**すべてのユーザー**の**すべてのアプリケーション**によって作成されるサブスクリプションです。</span><span class="sxs-lookup"><span data-stu-id="dae6c-150">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dae6c-151">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dae6c-151">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dae6c-152">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="dae6c-152">Optional query parameters</span></span>

<span data-ttu-id="dae6c-153">このメソッドは、応答をカスタマイズするために[OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="dae6c-153">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dae6c-154">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dae6c-154">Request headers</span></span>

| <span data-ttu-id="dae6c-155">名前</span><span class="sxs-lookup"><span data-stu-id="dae6c-155">Name</span></span>       | <span data-ttu-id="dae6c-156">型</span><span class="sxs-lookup"><span data-stu-id="dae6c-156">Type</span></span> | <span data-ttu-id="dae6c-157">説明</span><span class="sxs-lookup"><span data-stu-id="dae6c-157">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="dae6c-158">Authorization</span><span class="sxs-lookup"><span data-stu-id="dae6c-158">Authorization</span></span>  | <span data-ttu-id="dae6c-159">string</span><span class="sxs-lookup"><span data-stu-id="dae6c-159">string</span></span>  | <span data-ttu-id="dae6c-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="dae6c-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dae6c-162">要求本文</span><span class="sxs-lookup"><span data-stu-id="dae6c-162">Request body</span></span>

<span data-ttu-id="dae6c-163">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="dae6c-163">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dae6c-164">応答</span><span class="sxs-lookup"><span data-stu-id="dae6c-164">Response</span></span>

<span data-ttu-id="dae6c-165">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文のオブジェクトの[サブスクリプション](../resources/subscription.md)の一覧です。</span><span class="sxs-lookup"><span data-stu-id="dae6c-165">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dae6c-166">例</span><span class="sxs-lookup"><span data-stu-id="dae6c-166">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dae6c-167">要求</span><span class="sxs-lookup"><span data-stu-id="dae6c-167">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions
```

##### <a name="response"></a><span data-ttu-id="dae6c-168">応答</span><span class="sxs-lookup"><span data-stu-id="dae6c-168">Response</span></span>

<span data-ttu-id="dae6c-169">ここでは、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="dae6c-169">Here's an an example of the response.</span></span>  <span data-ttu-id="dae6c-170">簡潔にするために切り捨てられます可能性があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="dae6c-170">Note that it may be truncated for brevity.</span></span>  <span data-ttu-id="dae6c-171">すべての要求の適切なプロパティがサポートされているし、呼び出し元のコンテキストは、実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dae6c-171">All supported properties appropriate for the request and the calling context will be returned from an actual call.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

<span data-ttu-id="dae6c-172">応答が含まれて、要求にデータの複数のページが返されるとき、 `@odata.nextLink` 、結果を管理するためのプロパティです。</span><span class="sxs-lookup"><span data-stu-id="dae6c-172">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="dae6c-173">詳細については、[アプリケーションでは、Microsoft Graph のページング データ](/graph/paging)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dae6c-173">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
