---
title: サブスクリプションのリスト作成
description: " 詳細については、以下のシナリオを参照してください。"
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 20aad712bc49f91bec58a67c0c66ef76bf4653e2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537091"
---
# <a name="list-subscriptions"></a><span data-ttu-id="634b4-103">サブスクリプションのリスト作成</span><span class="sxs-lookup"><span data-stu-id="634b4-103">List subscriptions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="634b4-104">webhook サブスクリプションの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="634b4-104">Retrieve a list of webhook subscriptions.</span></span> <span data-ttu-id="634b4-105">応答の内容は、アプリが呼び出しているコンテキストによって異なります。詳細については、以下のシナリオを参照してください。</span><span class="sxs-lookup"><span data-stu-id="634b4-105">The content of the response depends on the context in which the app is calling; see the scenarios below for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="634b4-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="634b4-106">Permissions</span></span>

<span data-ttu-id="634b4-107">この API は、次のアクセス許可のスコープをサポートしています。アクセス許可の選択方法を含む詳細については、「 [permissions](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="634b4-107">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="634b4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="634b4-108">Permission type</span></span>  | <span data-ttu-id="634b4-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="634b4-109">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="634b4-110">[委任](/graph/auth-v2-user)された(職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="634b4-110">[Delegated](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="634b4-111">サブスクリプションまたはサブスクリプションを[作成](subscription-post-subscriptions.md)するために必要なアクセス許可。 All (下を参照)。</span><span class="sxs-lookup"><span data-stu-id="634b4-111">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="634b4-112">[委任](/graph/auth-v2-user)された(個人 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="634b4-112">[Delegated](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="634b4-113">サブスクリプションまたはサブスクリプションを[作成](subscription-post-subscriptions.md)するために必要なアクセス許可。 All (下を参照)。</span><span class="sxs-lookup"><span data-stu-id="634b4-113">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="634b4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="634b4-114">Application</span></span>](/graph/auth-v2-service) | <span data-ttu-id="634b4-115">[サブスクリプションを作成](subscription-post-subscriptions.md)するために必要なアクセス許可。</span><span class="sxs-lookup"><span data-stu-id="634b4-115">Permission required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="634b4-116">応答の結果は、呼び出し元アプリのコンテキストに基づいています。</span><span class="sxs-lookup"><span data-stu-id="634b4-116">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="634b4-117">一般的なシナリオの概要を次に示します。</span><span class="sxs-lookup"><span data-stu-id="634b4-117">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="634b4-118">基本的なシナリオ</span><span class="sxs-lookup"><span data-stu-id="634b4-118">Basic scenarios</span></span>

<span data-ttu-id="634b4-119">最も一般的には、アプリケーションは、現在サインインしているユーザーまたはディレクトリ内のすべてのユーザーに対して最初に作成されたサブスクリプションを取得したいと考えています (職場または学校のアカウント)。</span><span class="sxs-lookup"><span data-stu-id="634b4-119">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="634b4-120">これらのシナリオでは、最初にサブスクリプションを作成するために使用されたアプリ以外の特別なアクセス許可は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="634b4-120">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="634b4-121">呼び出し元アプリのコンテキスト</span><span class="sxs-lookup"><span data-stu-id="634b4-121">Context of the calling app</span></span> | <span data-ttu-id="634b4-122">応答の内容</span><span class="sxs-lookup"><span data-stu-id="634b4-122">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="634b4-123">アプリは、サインインしているユーザーの代わりに呼び出しを行います (委任されたアクセス許可)。</span><span class="sxs-lookup"><span data-stu-id="634b4-123">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="634b4-124">/</span><span class="sxs-lookup"><span data-stu-id="634b4-124">-and-</span></span><br/><span data-ttu-id="634b4-125">アプリには、[サブスクリプションを作成](subscription-post-subscriptions.md)するために必要な元のアクセス許可があります。</span><span class="sxs-lookup"><span data-stu-id="634b4-125">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="634b4-126">注: これは、個人用の Microsoft アカウントと職場/学校のアカウントの両方に適用されます。</span><span class="sxs-lookup"><span data-stu-id="634b4-126">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="634b4-127">サインインしているユーザーに対してのみ、**このアプリ**によって作成されたサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="634b4-127">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="634b4-128">アプリは自身の代わりに呼び出しをしています (アプリケーションアクセス許可)。</span><span class="sxs-lookup"><span data-stu-id="634b4-128">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="634b4-129">/</span><span class="sxs-lookup"><span data-stu-id="634b4-129">-and-</span></span><br/><span data-ttu-id="634b4-130">アプリには、[サブスクリプションを作成](subscription-post-subscriptions.md)するために必要な元のアクセス許可があります。</span><span class="sxs-lookup"><span data-stu-id="634b4-130">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="634b4-131">注: これは、職場または学校のアカウントにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="634b4-131">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="634b4-132">**このアプリ**によって自分用またはディレクトリ内のユーザー用に作成されたサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="634b4-132">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="634b4-133">高度なシナリオ</span><span class="sxs-lookup"><span data-stu-id="634b4-133">Advanced scenarios</span></span>

<span data-ttu-id="634b4-134">場合によっては、他のアプリによって作成されたサブスクリプションをアプリで取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="634b4-134">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="634b4-135">たとえば、ユーザーは、任意のアプリによって作成されたすべてのサブスクリプションを自分に代わって表示したいと考えています。</span><span class="sxs-lookup"><span data-stu-id="634b4-135">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="634b4-136">または、管理者がディレクトリ内のすべてのアプリからのすべてのサブスクリプションを表示する必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="634b4-136">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="634b4-137">このようなシナリオでは、委任されたアクセス許可のサブスクリプションが必要です。</span><span class="sxs-lookup"><span data-stu-id="634b4-137">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="634b4-138">呼び出し元アプリのコンテキスト</span><span class="sxs-lookup"><span data-stu-id="634b4-138">Context of the calling app</span></span> | <span data-ttu-id="634b4-139">応答の内容</span><span class="sxs-lookup"><span data-stu-id="634b4-139">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="634b4-140">アプリは、サインインしているユーザーの代わりに呼び出しを行います (委任されたアクセス許可)。</span><span class="sxs-lookup"><span data-stu-id="634b4-140">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="634b4-141">*ユーザーが管理者ではない*。</span><span class="sxs-lookup"><span data-stu-id="634b4-141">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="634b4-142">/</span><span class="sxs-lookup"><span data-stu-id="634b4-142">-and-</span></span><br/><span data-ttu-id="634b4-143">アプリには、アクセス許可のサブスクリプションがあります。 All</span><span class="sxs-lookup"><span data-stu-id="634b4-143">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="634b4-144">注: これは、個人用の Microsoft アカウントと職場/学校のアカウントの両方に適用されます。</span><span class="sxs-lookup"><span data-stu-id="634b4-144">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="634b4-145">サインインしているユーザーに対してのみ、**そのアプリ**によって作成されたサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="634b4-145">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="634b4-146">アプリは、サインインしているユーザーの代わりに呼び出しを行います (委任されたアクセス許可)。</span><span class="sxs-lookup"><span data-stu-id="634b4-146">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="634b4-147">*ユーザーが管理者*である。</span><span class="sxs-lookup"><span data-stu-id="634b4-147">*The user is an admin*.</span></span><br/><span data-ttu-id="634b4-148">/</span><span class="sxs-lookup"><span data-stu-id="634b4-148">-and-</span></span><br/><span data-ttu-id="634b4-149">アプリには、アクセス許可のサブスクリプションがあります。 All</span><span class="sxs-lookup"><span data-stu-id="634b4-149">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="634b4-150">注: これは、職場または学校のアカウントにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="634b4-150">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="634b4-151">ディレクトリ内の**すべてのユーザー**について、**任意のアプリ**によって作成されたサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="634b4-151">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="634b4-152">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="634b4-152">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="634b4-153">省略可能なクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="634b4-153">Optional query parameters</span></span>

<span data-ttu-id="634b4-154">このメソッドは、応答をカスタマイズするための[OData クエリパラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="634b4-154">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="634b4-155">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="634b4-155">Request headers</span></span>

| <span data-ttu-id="634b4-156">名前</span><span class="sxs-lookup"><span data-stu-id="634b4-156">Name</span></span>       | <span data-ttu-id="634b4-157">型</span><span class="sxs-lookup"><span data-stu-id="634b4-157">Type</span></span> | <span data-ttu-id="634b4-158">説明</span><span class="sxs-lookup"><span data-stu-id="634b4-158">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="634b4-159">Authorization</span><span class="sxs-lookup"><span data-stu-id="634b4-159">Authorization</span></span>  | <span data-ttu-id="634b4-160">string</span><span class="sxs-lookup"><span data-stu-id="634b4-160">string</span></span>  | <span data-ttu-id="634b4-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="634b4-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="634b4-163">要求本文</span><span class="sxs-lookup"><span data-stu-id="634b4-163">Request body</span></span>

<span data-ttu-id="634b4-164">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="634b4-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="634b4-165">応答</span><span class="sxs-lookup"><span data-stu-id="634b4-165">Response</span></span>

<span data-ttu-id="634b4-166">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[subscription](../resources/subscription.md)オブジェクトのリストを返します。</span><span class="sxs-lookup"><span data-stu-id="634b4-166">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="634b4-167">例</span><span class="sxs-lookup"><span data-stu-id="634b4-167">Example</span></span>

##### <a name="request"></a><span data-ttu-id="634b4-168">要求</span><span class="sxs-lookup"><span data-stu-id="634b4-168">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions
```

##### <a name="response"></a><span data-ttu-id="634b4-169">応答</span><span class="sxs-lookup"><span data-stu-id="634b4-169">Response</span></span>

<span data-ttu-id="634b4-170">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="634b4-170">Here is an example of the response.</span></span> <span data-ttu-id="634b4-171">注: 簡潔にするために、ここに示す応答は切り捨てられる場合があります。</span><span class="sxs-lookup"><span data-stu-id="634b4-171">Note: The response shown here may be truncated for brevity.</span></span> <span data-ttu-id="634b4-172">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="634b4-172">All of the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="634b4-173">要求が複数のデータページを返す場合、応答には`@odata.nextLink`結果を管理するためのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="634b4-173">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="634b4-174">詳細については、「[アプリで Microsoft Graph データをページング](/graph/paging)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="634b4-174">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
