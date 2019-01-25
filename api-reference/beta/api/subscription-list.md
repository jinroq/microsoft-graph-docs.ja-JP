---
title: リストの購読
description: " 詳細については以下のシナリオを参照してください。"
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 20aad712bc49f91bec58a67c0c66ef76bf4653e2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510982"
---
# <a name="list-subscriptions"></a><span data-ttu-id="11e47-103">リストの購読</span><span class="sxs-lookup"><span data-stu-id="11e47-103">List subscriptions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11e47-104">Webhook サブスクリプションの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="11e47-104">Retrieve a list of webhook subscriptions.</span></span> <span data-ttu-id="11e47-105">応答の内容では、アプリケーションを呼び出す; コンテキストによって異なります。詳細については以下のシナリオを参照してください。</span><span class="sxs-lookup"><span data-stu-id="11e47-105">The content of the response depends on the context in which the app is calling; see the scenarios below for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="11e47-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="11e47-106">Permissions</span></span>

<span data-ttu-id="11e47-107">この API には、次のアクセス許可のスコープがサポートされています。アクセス許可] を選択する方法などの詳細については、[アクセス許可](/graph/permissions-reference)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="11e47-107">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11e47-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="11e47-108">Permission type</span></span>  | <span data-ttu-id="11e47-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="11e47-109">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="11e47-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="11e47-110">[Delegated](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="11e47-111">[サブスクリプションを作成](subscription-post-subscriptions.md)または Subscription.Read.All (下記参照) に必要なアクセスを許可します。</span><span class="sxs-lookup"><span data-stu-id="11e47-111">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="11e47-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="11e47-112">[Delegated](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="11e47-113">[サブスクリプションを作成](subscription-post-subscriptions.md)または Subscription.Read.All (下記参照) に必要なアクセスを許可します。</span><span class="sxs-lookup"><span data-stu-id="11e47-113">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="11e47-114">Application</span><span class="sxs-lookup"><span data-stu-id="11e47-114">Application</span></span>](/graph/auth-v2-service) | <span data-ttu-id="11e47-115">[サブスクリプションを作成](subscription-post-subscriptions.md)するために必要なアクセスを許可します。</span><span class="sxs-lookup"><span data-stu-id="11e47-115">Permission required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="11e47-116">応答の結果は、呼び出し元のアプリケーションのコンテキストに基づいています。</span><span class="sxs-lookup"><span data-stu-id="11e47-116">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="11e47-117">以下は、一般的なシナリオの概要です。</span><span class="sxs-lookup"><span data-stu-id="11e47-117">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="11e47-118">基本的なシナリオ</span><span class="sxs-lookup"><span data-stu-id="11e47-118">Basic scenarios</span></span>

<span data-ttu-id="11e47-119">ほとんどの場合、アプリケーションは、最初に作成された、現在サインインしているユーザーやディレクトリ (仕事/学校のアカウント) のすべてのユーザーのサブスクリプションを取得しようとします。</span><span class="sxs-lookup"><span data-stu-id="11e47-119">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="11e47-120">これらのシナリオは不要のもの以外の特殊なアクセス許可のサブスクリプションを作成する最初に使用するアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="11e47-120">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="11e47-121">呼び出し元のアプリケーションのコンテキスト</span><span class="sxs-lookup"><span data-stu-id="11e47-121">Context of the calling app</span></span> | <span data-ttu-id="11e47-122">応答が含まれています</span><span class="sxs-lookup"><span data-stu-id="11e47-122">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="11e47-123">サインインしているユーザー (委任されたアクセス許可) のため、アプリケーションを呼び出しています。</span><span class="sxs-lookup"><span data-stu-id="11e47-123">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="11e47-124">And</span><span class="sxs-lookup"><span data-stu-id="11e47-124">-and-</span></span><br/><span data-ttu-id="11e47-125">アプリケーションでは、[サブスクリプションを作成](subscription-post-subscriptions.md)するために必要な元の権限を持っています。</span><span class="sxs-lookup"><span data-stu-id="11e47-125">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="11e47-126">注意: 個人用の Microsoft アカウントとアカウントの仕事/学校の両方に適用します。</span><span class="sxs-lookup"><span data-stu-id="11e47-126">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="11e47-127">サブスクリプションは、サインインしているユーザーに対してのみ、**このアプリケーション**によって作成されました。</span><span class="sxs-lookup"><span data-stu-id="11e47-127">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="11e47-128">自体 (アプリケーションのアクセス許可) のため、アプリケーションを呼び出しています。</span><span class="sxs-lookup"><span data-stu-id="11e47-128">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="11e47-129">And</span><span class="sxs-lookup"><span data-stu-id="11e47-129">-and-</span></span><br/><span data-ttu-id="11e47-130">アプリケーションでは、[サブスクリプションを作成](subscription-post-subscriptions.md)するために必要な元の権限を持っています。</span><span class="sxs-lookup"><span data-stu-id="11e47-130">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="11e47-131">注意: 仕事/学校のアカウントのみに適用します。</span><span class="sxs-lookup"><span data-stu-id="11e47-131">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="11e47-132">自体やディレクトリ内のすべてのユーザーに、**このアプリケーション**によって作成されたサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="11e47-132">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="11e47-133">高度なシナリオ</span><span class="sxs-lookup"><span data-stu-id="11e47-133">Advanced scenarios</span></span>

<span data-ttu-id="11e47-134">場合によっては、アプリケーションは、他のアプリケーションによって作成されたサブスクリプションを取得しようとします。</span><span class="sxs-lookup"><span data-stu-id="11e47-134">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="11e47-135">たとえば、ユーザーは代わりに他のアプリケーションによって作成されたすべてのサブスクリプションを参照してください希望しています。</span><span class="sxs-lookup"><span data-stu-id="11e47-135">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="11e47-136">または、管理者はそのディレクトリ内のすべてのアプリケーションからのすべてのサブスクリプションを参照してくださいすることがあります。</span><span class="sxs-lookup"><span data-stu-id="11e47-136">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="11e47-137">このような状況では、Subscription.Read.All の委任されたアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="11e47-137">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="11e47-138">呼び出し元のアプリケーションのコンテキスト</span><span class="sxs-lookup"><span data-stu-id="11e47-138">Context of the calling app</span></span> | <span data-ttu-id="11e47-139">応答が含まれています</span><span class="sxs-lookup"><span data-stu-id="11e47-139">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="11e47-140">サインインしているユーザー (委任されたアクセス許可) のため、アプリケーションを呼び出しています。</span><span class="sxs-lookup"><span data-stu-id="11e47-140">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="11e47-141">*ユーザーは管理者以外*は。</span><span class="sxs-lookup"><span data-stu-id="11e47-141">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="11e47-142">And</span><span class="sxs-lookup"><span data-stu-id="11e47-142">-and-</span></span><br/><span data-ttu-id="11e47-143">アプリには、アクセス許可が Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="11e47-143">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="11e47-144">注意: 個人用の Microsoft アカウントとアカウントの仕事/学校の両方に適用します。</span><span class="sxs-lookup"><span data-stu-id="11e47-144">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="11e47-145">サブスクリプションは、サインインしているユーザーに対してのみ **、アプリケーション**によって作成されました。</span><span class="sxs-lookup"><span data-stu-id="11e47-145">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="11e47-146">サインインしているユーザー (委任されたアクセス許可) のため、アプリケーションを呼び出しています。</span><span class="sxs-lookup"><span data-stu-id="11e47-146">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="11e47-147">*ユーザーは管理者*です。</span><span class="sxs-lookup"><span data-stu-id="11e47-147">*The user is an admin*.</span></span><br/><span data-ttu-id="11e47-148">And</span><span class="sxs-lookup"><span data-stu-id="11e47-148">-and-</span></span><br/><span data-ttu-id="11e47-149">アプリには、アクセス許可が Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="11e47-149">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="11e47-150">注意: 仕事/学校のアカウントのみに適用します。</span><span class="sxs-lookup"><span data-stu-id="11e47-150">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="11e47-151">ディレクトリ内の**すべてのユーザー**の**すべてのアプリケーション**によって作成されるサブスクリプションです。</span><span class="sxs-lookup"><span data-stu-id="11e47-151">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11e47-152">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="11e47-152">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="11e47-153">省略可能なクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="11e47-153">Optional query parameters</span></span>

<span data-ttu-id="11e47-154">このメソッドは、応答をカスタマイズするために[OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="11e47-154">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="11e47-155">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="11e47-155">Request headers</span></span>

| <span data-ttu-id="11e47-156">名前</span><span class="sxs-lookup"><span data-stu-id="11e47-156">Name</span></span>       | <span data-ttu-id="11e47-157">型</span><span class="sxs-lookup"><span data-stu-id="11e47-157">Type</span></span> | <span data-ttu-id="11e47-158">説明</span><span class="sxs-lookup"><span data-stu-id="11e47-158">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="11e47-159">Authorization</span><span class="sxs-lookup"><span data-stu-id="11e47-159">Authorization</span></span>  | <span data-ttu-id="11e47-160">string</span><span class="sxs-lookup"><span data-stu-id="11e47-160">string</span></span>  | <span data-ttu-id="11e47-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="11e47-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11e47-163">要求本文</span><span class="sxs-lookup"><span data-stu-id="11e47-163">Request body</span></span>

<span data-ttu-id="11e47-164">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="11e47-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11e47-165">応答</span><span class="sxs-lookup"><span data-stu-id="11e47-165">Response</span></span>

<span data-ttu-id="11e47-166">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文のオブジェクトの[サブスクリプション](../resources/subscription.md)の一覧です。</span><span class="sxs-lookup"><span data-stu-id="11e47-166">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11e47-167">例</span><span class="sxs-lookup"><span data-stu-id="11e47-167">Example</span></span>

##### <a name="request"></a><span data-ttu-id="11e47-168">要求</span><span class="sxs-lookup"><span data-stu-id="11e47-168">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions
```

##### <a name="response"></a><span data-ttu-id="11e47-169">応答</span><span class="sxs-lookup"><span data-stu-id="11e47-169">Response</span></span>

<span data-ttu-id="11e47-170">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="11e47-170">Here is an example of the response.</span></span> <span data-ttu-id="11e47-171">注: ここに示す応答は簡潔にするためにあります。</span><span class="sxs-lookup"><span data-stu-id="11e47-171">Note: The response shown here may be truncated for brevity.</span></span> <span data-ttu-id="11e47-172">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="11e47-172">All of the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

<span data-ttu-id="11e47-173">応答が含まれて、要求にデータの複数のページが返されるとき、 `@odata.nextLink` 、結果を管理するためのプロパティです。</span><span class="sxs-lookup"><span data-stu-id="11e47-173">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="11e47-174">詳細については、[アプリケーションでは、Microsoft Graph のページング データ](/graph/paging)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="11e47-174">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
