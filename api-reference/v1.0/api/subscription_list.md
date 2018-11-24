# <a name="list-subscriptions"></a><span data-ttu-id="c10ac-101">リストの購読</span><span class="sxs-lookup"><span data-stu-id="c10ac-101">List subscriptions</span></span>

<span data-ttu-id="c10ac-102">プロパティとアプリケーション ID、ユーザー、およびテナントのユーザーのロールに基づいて、webhook サブスクリプションの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="c10ac-102">Retrieve the properties and relationships of webhook subscriptions, based on the app ID, the user, and the user's role with a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="c10ac-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c10ac-103">Permissions</span></span>

<span data-ttu-id="c10ac-104">この API には、次のアクセス許可のスコープがサポートされています。アクセス許可] を選択する方法などの詳細については、[アクセス許可](../../../concepts/permissions_reference.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c10ac-104">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="c10ac-105">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c10ac-105">Permission type</span></span>  | <span data-ttu-id="c10ac-106">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c10ac-106">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="c10ac-107">[委任されたアクセス許可](../../../concepts/auth_v2_user.md)(職場、学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c10ac-107">[Delegated permission](../../../concepts/auth_v2_user.md) (work or school account)</span></span> | <span data-ttu-id="c10ac-108">[サブスクリプションを作成](subscription_post_subscriptions.md)または Subscription.Read.All (下記参照) に必要なロールです。</span><span class="sxs-lookup"><span data-stu-id="c10ac-108">Role required to [create subscription](subscription_post_subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="c10ac-109">[委任されたアクセス許可](../../../concepts/auth_v2_user.md)(個人用の Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c10ac-109">[Delegated permission](../../../concepts/auth_v2_user.md) (personal Microsoft account)</span></span> | <span data-ttu-id="c10ac-110">[サブスクリプションを作成](subscription_post_subscriptions.md)または Subscription.Read.All (下記参照) に必要なロールです。</span><span class="sxs-lookup"><span data-stu-id="c10ac-110">Role required to [create subscription](subscription_post_subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="c10ac-111">アプリケーションのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="c10ac-111">Application permission</span></span>](../../../concepts/auth_v2_service.md) | <span data-ttu-id="c10ac-112">[サブスクリプションを作成](subscription_post_subscriptions.md)するために必要なロールです。</span><span class="sxs-lookup"><span data-stu-id="c10ac-112">Role required to [create subscription](subscription_post_subscriptions.md).</span></span> |

<span data-ttu-id="c10ac-113">応答の結果は、呼び出し元のアプリケーションのコンテキストに基づいています。</span><span class="sxs-lookup"><span data-stu-id="c10ac-113">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="c10ac-114">以下は、一般的なシナリオの概要です。</span><span class="sxs-lookup"><span data-stu-id="c10ac-114">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="c10ac-115">基本的なシナリオ</span><span class="sxs-lookup"><span data-stu-id="c10ac-115">Basic scenarios</span></span>

<span data-ttu-id="c10ac-116">ほとんどの場合、アプリケーションは、最初に作成された、現在サインインしているユーザーやディレクトリ (仕事/学校のアカウント) のすべてのユーザーのサブスクリプションを取得しようとします。</span><span class="sxs-lookup"><span data-stu-id="c10ac-116">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="c10ac-117">これらのシナリオは不要のもの以外の特殊なアクセス許可のサブスクリプションを作成する最初に使用するアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="c10ac-117">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="c10ac-118">呼び出し元のアプリケーションのコンテキスト</span><span class="sxs-lookup"><span data-stu-id="c10ac-118">Context of the calling app</span></span> | <span data-ttu-id="c10ac-119">応答が含まれています</span><span class="sxs-lookup"><span data-stu-id="c10ac-119">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="c10ac-120">サインインしているユーザー (委任されたアクセス許可) のため、アプリケーションを呼び出しています。</span><span class="sxs-lookup"><span data-stu-id="c10ac-120">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="c10ac-121">- と -</span><span class="sxs-lookup"><span data-stu-id="c10ac-121">-and-</span></span><br/><span data-ttu-id="c10ac-122">アプリケーションでは、[サブスクリプションを作成](subscription_post_subscriptions.md)するために必要な元の権限を持っています。</span><span class="sxs-lookup"><span data-stu-id="c10ac-122">App has the original permission required to [create the subscription](subscription_post_subscriptions.md).</span></span><br/><br/><span data-ttu-id="c10ac-123">注意: 個人用の Microsoft アカウントとアカウントの仕事/学校の両方に適用します。</span><span class="sxs-lookup"><span data-stu-id="c10ac-123">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="c10ac-124">サブスクリプションは、サインインしているユーザーに対してのみ、**このアプリケーション**によって作成されました。</span><span class="sxs-lookup"><span data-stu-id="c10ac-124">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="c10ac-125">自体 (アプリケーションのアクセス許可) のため、アプリケーションを呼び出しています。</span><span class="sxs-lookup"><span data-stu-id="c10ac-125">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="c10ac-126">- と -</span><span class="sxs-lookup"><span data-stu-id="c10ac-126">-and-</span></span><br/><span data-ttu-id="c10ac-127">アプリケーションでは、[サブスクリプションを作成](subscription_post_subscriptions.md)するために必要な元の権限を持っています。</span><span class="sxs-lookup"><span data-stu-id="c10ac-127">App has the original permission required to [create the subscription](subscription_post_subscriptions.md).</span></span><br/><br/><span data-ttu-id="c10ac-128">注意: 仕事/学校のアカウントのみに適用します。</span><span class="sxs-lookup"><span data-stu-id="c10ac-128">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="c10ac-129">自体やディレクトリ内のすべてのユーザーに、**このアプリケーション**によって作成されたサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="c10ac-129">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="c10ac-130">高度なシナリオ</span><span class="sxs-lookup"><span data-stu-id="c10ac-130">Advanced scenarios</span></span>

<span data-ttu-id="c10ac-131">場合によっては、アプリケーションは、他のアプリケーションによって作成されたサブスクリプションを取得しようとします。</span><span class="sxs-lookup"><span data-stu-id="c10ac-131">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="c10ac-132">たとえば、ユーザーは代わりに他のアプリケーションによって作成されたすべてのサブスクリプションを参照してください希望しています。</span><span class="sxs-lookup"><span data-stu-id="c10ac-132">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="c10ac-133">または、管理者はそのディレクトリ内のすべてのアプリケーションからのすべてのサブスクリプションを参照してくださいすることがあります。</span><span class="sxs-lookup"><span data-stu-id="c10ac-133">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="c10ac-134">このような状況では、Subscription.Read.All の委任されたアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="c10ac-134">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="c10ac-135">呼び出し元のアプリケーションのコンテキスト</span><span class="sxs-lookup"><span data-stu-id="c10ac-135">Context of the calling app</span></span> | <span data-ttu-id="c10ac-136">応答が含まれています</span><span class="sxs-lookup"><span data-stu-id="c10ac-136">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="c10ac-137">サインインしているユーザー (委任されたアクセス許可) のため、アプリケーションを呼び出しています。</span><span class="sxs-lookup"><span data-stu-id="c10ac-137">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="c10ac-138">*ユーザーは管理者以外*は。</span><span class="sxs-lookup"><span data-stu-id="c10ac-138">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="c10ac-139">- と -</span><span class="sxs-lookup"><span data-stu-id="c10ac-139">-and-</span></span><br/><span data-ttu-id="c10ac-140">アプリには、アクセス許可が Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="c10ac-140">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="c10ac-141">注意: 個人用の Microsoft アカウントとアカウントの仕事/学校の両方に適用します。</span><span class="sxs-lookup"><span data-stu-id="c10ac-141">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="c10ac-142">サブスクリプションは、サインインしているユーザーに対してのみ **、アプリケーション**によって作成されました。</span><span class="sxs-lookup"><span data-stu-id="c10ac-142">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="c10ac-143">サインインしているユーザー (委任されたアクセス許可) のため、アプリケーションを呼び出しています。</span><span class="sxs-lookup"><span data-stu-id="c10ac-143">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="c10ac-144">*ユーザーは管理者*です。</span><span class="sxs-lookup"><span data-stu-id="c10ac-144">*The user is an admin*.</span></span><br/><span data-ttu-id="c10ac-145">- と -</span><span class="sxs-lookup"><span data-stu-id="c10ac-145">-and-</span></span><br/><span data-ttu-id="c10ac-146">アプリには、アクセス許可が Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="c10ac-146">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="c10ac-147">注意: 仕事/学校のアカウントのみに適用します。</span><span class="sxs-lookup"><span data-stu-id="c10ac-147">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="c10ac-148">ディレクトリ内の**すべてのユーザー**の**すべてのアプリケーション**によって作成されるサブスクリプションです。</span><span class="sxs-lookup"><span data-stu-id="c10ac-148">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c10ac-149">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c10ac-149">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c10ac-150">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c10ac-150">Optional query parameters</span></span>

<span data-ttu-id="c10ac-151">このメソッドは、応答をカスタマイズするために[OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="c10ac-151">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c10ac-152">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c10ac-152">Request headers</span></span>

| <span data-ttu-id="c10ac-153">名前</span><span class="sxs-lookup"><span data-stu-id="c10ac-153">Name</span></span>       | <span data-ttu-id="c10ac-154">型</span><span class="sxs-lookup"><span data-stu-id="c10ac-154">Type</span></span> | <span data-ttu-id="c10ac-155">説明</span><span class="sxs-lookup"><span data-stu-id="c10ac-155">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c10ac-156">Authorization</span><span class="sxs-lookup"><span data-stu-id="c10ac-156">Authorization</span></span>  | <span data-ttu-id="c10ac-157">string</span><span class="sxs-lookup"><span data-stu-id="c10ac-157">string</span></span>  | <span data-ttu-id="c10ac-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c10ac-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c10ac-160">要求本文</span><span class="sxs-lookup"><span data-stu-id="c10ac-160">Request body</span></span>

<span data-ttu-id="c10ac-161">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c10ac-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c10ac-162">応答</span><span class="sxs-lookup"><span data-stu-id="c10ac-162">Response</span></span>

<span data-ttu-id="c10ac-163">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文のオブジェクトの[サブスクリプション](../resources/subscription.md)の一覧です。</span><span class="sxs-lookup"><span data-stu-id="c10ac-163">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c10ac-164">例</span><span class="sxs-lookup"><span data-stu-id="c10ac-164">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c10ac-165">要求</span><span class="sxs-lookup"><span data-stu-id="c10ac-165">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions
```

##### <a name="response"></a><span data-ttu-id="c10ac-166">応答</span><span class="sxs-lookup"><span data-stu-id="c10ac-166">Response</span></span>

<span data-ttu-id="c10ac-167">ここでは、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c10ac-167">Here's an an example of the response.</span></span>  <span data-ttu-id="c10ac-168">簡潔にするために切り捨てられます可能性があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="c10ac-168">Note that it may be truncated for brevity.</span></span>  <span data-ttu-id="c10ac-169">すべての要求の適切なプロパティがサポートされているし、呼び出し元のコンテキストは、実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c10ac-169">All supported properties appropriate for the request and the calling context will be returned from an actual call.</span></span>

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

<span data-ttu-id="c10ac-170">応答が含まれて、要求にデータの複数のページが返されるとき、 `@odata.nextLink` 、結果を管理するためのプロパティです。</span><span class="sxs-lookup"><span data-stu-id="c10ac-170">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="c10ac-171">詳細については、[アプリケーションでは、Microsoft Graph のページング データ](../../../concepts/paging.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c10ac-171">To learn more, see [Paging Microsoft Graph data in your app](../../../concepts/paging.md).</span></span>
