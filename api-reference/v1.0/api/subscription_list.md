# <a name="list-subscriptions"></a><span data-ttu-id="ed926-101">サブスクリプションのリストアップ</span><span class="sxs-lookup"><span data-stu-id="ed926-101">List current subscriptions</span></span>

<span data-ttu-id="ed926-102">アプリ ID、ユーザー、テナントでのユーザーのロールに基づいて、Web フックへのサブスクリプションのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="ed926-102">Retrieve the properties and relationships of webhook subscriptions, based on the app ID, the user, and the user's role with a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed926-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ed926-103">Permissions</span></span>

<span data-ttu-id="ed926-104">この API では、次のアクセス許可の範囲をサポートしています。アクセス許可の選択方法などの詳細については、[アクセス許可](../../../concepts/permissions_reference.md) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ed926-104">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="ed926-105">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ed926-105">Permission type</span></span>  | <span data-ttu-id="ed926-106">アクセス許可 (権限が最小のものから最大のものへ)</span><span class="sxs-lookup"><span data-stu-id="ed926-106">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="ed926-107">[委任](../../../concepts/auth_v2_user.md) (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ed926-107">Delegated (work or school account)</span></span> | <span data-ttu-id="ed926-108"> [サブスクリプションを作成](subscription_get.md) するのに、または Subscriptions.Read.All (下記参照) に必要なロールです。</span><span class="sxs-lookup"><span data-stu-id="ed926-108">Role required to [create subscription](subscription_get.md) or Subscriptions.Read.All (see below).</span></span> |
| <span data-ttu-id="ed926-109">[委任](../../../concepts/auth_v2_user.md) (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ed926-109">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed926-110"> [サブスクリプションを作成](./subscription_get.md) するのに、または Subscriptions.Read.All (下記参照) に必要なロールです。</span><span class="sxs-lookup"><span data-stu-id="ed926-110">Role required to [create subscription](./subscription_get.md) or Subscriptions.Read.All (see below).</span></span> |
| [<span data-ttu-id="ed926-111">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ed926-111">Application</span></span>](../../../concepts/auth_v2_service.md) | <span data-ttu-id="ed926-112"> [サブスクリプションを作成](./subscription_get.md) するために必要なロールです。</span><span class="sxs-lookup"><span data-stu-id="ed926-112">Role required to [create subscription](./subscription_get.md).</span></span> |

<span data-ttu-id="ed926-113">応答の結果は、呼び出し元のアプリのコンテキストに基づいています。</span><span class="sxs-lookup"><span data-stu-id="ed926-113">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="ed926-114">以下は、一般的なシナリオの概要です。</span><span class="sxs-lookup"><span data-stu-id="ed926-114">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="ed926-115">基本的なシナリオ</span><span class="sxs-lookup"><span data-stu-id="ed926-115">Basic planning scenarios</span></span>

<span data-ttu-id="ed926-116">ほとんどの場合、アプリケーションは、サインインしているユーザー向け、またはディレクトリ内のユーザー（仕事/学校のアカウント）向けに最初に作成したサブスクリプションを取得しようとします。</span><span class="sxs-lookup"><span data-stu-id="ed926-116">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="ed926-117">これらのシナリオでは、サブスクリプションを作成するのにアプリが最初に使用したものを越える、特殊なアクセス許可を必要としません。</span><span class="sxs-lookup"><span data-stu-id="ed926-117">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="ed926-118">呼び出し元のアプリのコンテキスト</span><span class="sxs-lookup"><span data-stu-id="ed926-118">Context of the calling app</span></span> | <span data-ttu-id="ed926-119">応答に含まれるもの</span><span class="sxs-lookup"><span data-stu-id="ed926-119">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="ed926-120">アプリはサインインしたユーザーの代理として呼び出しています（委任されたアクセス許可）。</span><span class="sxs-lookup"><span data-stu-id="ed926-120">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="ed926-121">および</span><span class="sxs-lookup"><span data-stu-id="ed926-121">and</span></span><br/><span data-ttu-id="ed926-122">アプリには、 [サブスクリプションを作成](subscription_post_subscriptions.md) するために必要なオリジナルのアクセス許可があります。</span><span class="sxs-lookup"><span data-stu-id="ed926-122">App has the original permission required to [create the subscription](subscription_post_subscriptions.md).</span></span><br/><br/><span data-ttu-id="ed926-123">注意: 個人用の Microsoft アカウントと仕事/学校のアカウントの両方に適用します。</span><span class="sxs-lookup"><span data-stu-id="ed926-123">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="ed926-124">**このアプリ** が作成したサブスクリプションは、サインインしているユーザーのみに有効です。</span><span class="sxs-lookup"><span data-stu-id="ed926-124">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="ed926-125">アプリは、アプリ自体の代理として呼び出しています（アプリケーション アクセス許可）</span><span class="sxs-lookup"><span data-stu-id="ed926-125">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="ed926-126">および</span><span class="sxs-lookup"><span data-stu-id="ed926-126">and</span></span><br/><span data-ttu-id="ed926-127">アプリには、 [サブスクリプションを作成](subscription_post_subscriptions.md) するために必要なオリジナルのアクセス許可があります。</span><span class="sxs-lookup"><span data-stu-id="ed926-127">App has the original permission required to [create the subscription](subscription_post_subscriptions.md).</span></span><br/><br/><span data-ttu-id="ed926-128">注意: 仕事/学校のアカウントのみに適用します。</span><span class="sxs-lookup"><span data-stu-id="ed926-128">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="ed926-129">**このアプリ** が作成したサブスクリプションは、アプリ自体またはディレクトリ内のユーザーのみに有効です。</span><span class="sxs-lookup"><span data-stu-id="ed926-129">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="ed926-130">高度なシナリオ</span><span class="sxs-lookup"><span data-stu-id="ed926-130">Advanced save scenarios</span></span>

<span data-ttu-id="ed926-131">場合によっては、アプリケーションは、他のアプリが作成したサブスクリプションを取得しようとします。</span><span class="sxs-lookup"><span data-stu-id="ed926-131">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="ed926-132">たとえば、あるユーザーが、アプリが作成したすべてのサブスクリプションを代理として閲覧しようとすることがあります。</span><span class="sxs-lookup"><span data-stu-id="ed926-132">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="ed926-133">または、管理者がディレクトリ内のすべてのアプリから、すべてのサブスクリプションを閲覧しようとするかもしれません。</span><span class="sxs-lookup"><span data-stu-id="ed926-133">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="ed926-134">このようなシナリオでは、委任されたアクセス許可 Subscription.Read.All が必要です。</span><span class="sxs-lookup"><span data-stu-id="ed926-134">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="ed926-135">呼び出し元のアプリのコンテキスト</span><span class="sxs-lookup"><span data-stu-id="ed926-135">Context of the calling app</span></span> | <span data-ttu-id="ed926-136">応答に含まれるもの</span><span class="sxs-lookup"><span data-stu-id="ed926-136">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="ed926-137">アプリはサインインしたユーザーの代理として呼び出しています（委任されたアクセス許可）。</span><span class="sxs-lookup"><span data-stu-id="ed926-137">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="ed926-138">*ユーザーは管理者ではありません*。</span><span class="sxs-lookup"><span data-stu-id="ed926-138">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="ed926-139">および</span><span class="sxs-lookup"><span data-stu-id="ed926-139">and</span></span><br/><span data-ttu-id="ed926-140">アプリには、アクセス許可 Subscription.Read.All があります。</span><span class="sxs-lookup"><span data-stu-id="ed926-140">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="ed926-141">注意: 個人用の Microsoft アカウントと仕事/学校のアカウントの両方に適用します。</span><span class="sxs-lookup"><span data-stu-id="ed926-141">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="ed926-142">**すべてのアプリ** が作成したサブスクリプションは、サインインしているユーザーのみに有効です。</span><span class="sxs-lookup"><span data-stu-id="ed926-142">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="ed926-143">アプリはサインインしたユーザーの代理として呼び出しています（委任されたアクセス許可）。</span><span class="sxs-lookup"><span data-stu-id="ed926-143">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="ed926-144">*ユーザーは管理者です*。</span><span class="sxs-lookup"><span data-stu-id="ed926-144">*The user is an admin*.</span></span><br/><span data-ttu-id="ed926-145">および</span><span class="sxs-lookup"><span data-stu-id="ed926-145">and</span></span><br/><span data-ttu-id="ed926-146">アプリには、アクセス許可 Subscription.Read.All があります。</span><span class="sxs-lookup"><span data-stu-id="ed926-146">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="ed926-147">注意: 仕事/学校のアカウントのみに適用します。</span><span class="sxs-lookup"><span data-stu-id="ed926-147">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="ed926-148">**すべてのアプリ** が作成したサブスクリプションは、ディレクトリ内の**すべてのユーザー** に対して有効です。</span><span class="sxs-lookup"><span data-stu-id="ed926-148">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed926-149">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ed926-149">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ed926-150">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ed926-150">Optional query parameters</span></span>

<span data-ttu-id="ed926-151">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="ed926-151">This method does not support the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed926-152">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed926-152">Request headers</span></span>

| <span data-ttu-id="ed926-153">名前</span><span class="sxs-lookup"><span data-stu-id="ed926-153">Name</span></span>       | <span data-ttu-id="ed926-154">型</span><span class="sxs-lookup"><span data-stu-id="ed926-154">Type</span></span> | <span data-ttu-id="ed926-155">説明</span><span class="sxs-lookup"><span data-stu-id="ed926-155">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ed926-156">承認</span><span class="sxs-lookup"><span data-stu-id="ed926-156">Authorization</span></span>  | <span data-ttu-id="ed926-157">string</span><span class="sxs-lookup"><span data-stu-id="ed926-157">string</span></span>  | <span data-ttu-id="ed926-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ed926-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed926-160">要求本文</span><span class="sxs-lookup"><span data-stu-id="ed926-160">Request body</span></span>

<span data-ttu-id="ed926-161">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ed926-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed926-162">応答</span><span class="sxs-lookup"><span data-stu-id="ed926-162">Response</span></span>

<span data-ttu-id="ed926-163">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文の [サブスクリプション](../resources/subscription.md) のリストを返します。</span><span class="sxs-lookup"><span data-stu-id="ed926-163">If successful, this method returns a `200 OK` response code and a collection of [enrollmentTroubleshootingEvent](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed926-164">例</span><span class="sxs-lookup"><span data-stu-id="ed926-164">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ed926-165">要求</span><span class="sxs-lookup"><span data-stu-id="ed926-165">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions
```

##### <a name="response"></a><span data-ttu-id="ed926-166">応答</span><span class="sxs-lookup"><span data-stu-id="ed926-166">Response</span></span>

<span data-ttu-id="ed926-167">応答の例をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="ed926-167">Here's an excerpt of the response:</span></span>  <span data-ttu-id="ed926-168">簡潔にするために切り詰められる可能性があることにご注意ください。</span><span class="sxs-lookup"><span data-stu-id="ed926-168">Note that it may be truncated for brevity.</span></span>  <span data-ttu-id="ed926-169">要求と呼び出しのコンテキストに適切なサポートされたプロパティはすべて、実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ed926-169">All supported properties appropriate for the request and the calling context will be returned from an actual call.</span></span>

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

<span data-ttu-id="ed926-170">要求が複数のページのデータを返す場合は、結果を管理するために応答には `@odata.nextLink` プロパティ含まれます。</span><span class="sxs-lookup"><span data-stu-id="ed926-170">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="ed926-171">詳細については、「[アプリで Microsoft Graph のデータをページングする](../../../concepts/paging.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ed926-171">To learn more, see [Paging Microsoft Graph data in your app](../../../concepts/paging.md).</span></span>
