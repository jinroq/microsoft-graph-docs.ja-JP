# <a name="update-settings"></a><span data-ttu-id="d4496-101">設定の更新</span><span class="sxs-lookup"><span data-stu-id="d4496-101">Update settings</span></span>

<span data-ttu-id="d4496-102">[設定](../resources/user_settings.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d4496-102">Update the properties of the [settings](../resources/user_settings.md) object.</span></span> <span data-ttu-id="d4496-103">同じ組織内のユーザーは、優先順位または組織のポリシーに基づいて、異なる設定を持つことができます。</span><span class="sxs-lookup"><span data-stu-id="d4496-103">Users in the same organization can have different settings based on their preference or on the organization policies.</span></span> <span data-ttu-id="d4496-104">ユーザーの現在の設定を取得、[現在のユーザー設定](user_get_settings.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d4496-104">To get the user current settings, see [current user settings](user_get_settings.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="d4496-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d4496-105">Permissions</span></span>

<span data-ttu-id="d4496-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d4496-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d4496-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d4496-108">Permission type</span></span>      | <span data-ttu-id="d4496-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d4496-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4496-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d4496-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d4496-111">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4496-111">User.ReadWrite, User.ReadWrite.All</span></span>   |
|<span data-ttu-id="d4496-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d4496-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4496-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4496-113">Not supported.</span></span>    |
|<span data-ttu-id="d4496-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d4496-114">Application</span></span> | <span data-ttu-id="d4496-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4496-115">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4496-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d4496-116">HTTP request</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/me/settings
```

<span data-ttu-id="d4496-117">'UserPrincipalName' は、ユーザー、または User.ReadWrite.All のアクセス許可を持つユーザーがアクセス可能なや、ユーザー id が要求されます。</span><span class="sxs-lookup"><span data-stu-id="d4496-117">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="d4496-118">詳細については、[アクセス許可](../../../concepts/permissions_reference.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d4496-118">To learn more, see [Permissions](../../../concepts/permissions_reference.md).</span></span> 

```http
PATCH https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}/settings/
```

## <a name="request-headers"></a><span data-ttu-id="d4496-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d4496-119">Request headers</span></span>

| <span data-ttu-id="d4496-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d4496-120">Header</span></span>       | <span data-ttu-id="d4496-121">値</span><span class="sxs-lookup"><span data-stu-id="d4496-121">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="d4496-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4496-122">Authorization</span></span>  | <span data-ttu-id="d4496-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d4496-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d4496-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d4496-125">Content-Type</span></span>  | <span data-ttu-id="d4496-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4496-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d4496-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d4496-127">Request body</span></span>

<span data-ttu-id="d4496-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="d4496-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d4496-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d4496-131">Property</span></span>     | <span data-ttu-id="d4496-132">型</span><span class="sxs-lookup"><span data-stu-id="d4496-132">Type</span></span>   |<span data-ttu-id="d4496-133">説明</span><span class="sxs-lookup"><span data-stu-id="d4496-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4496-134">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="d4496-134">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="d4496-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4496-135">Boolean</span></span>|<span data-ttu-id="d4496-136">True を設定するには、 [Trending](../../beta/resources/insights_trending.md) API およびユーザーの Office についてのドキュメントへのアクセスを無効にする代理人へのアクセスは無効にします。</span><span class="sxs-lookup"><span data-stu-id="d4496-136">Set to true do disable delegate access to the [Trending](../../beta/resources/insights_trending.md) API and to disable access to documents in Office Delve for the user.</span></span> <span data-ttu-id="d4496-137">Office 365 に表示されるコンテンツの関連性に影響を与えるも true に設定 - 候補のサイトでは、SharePoint のホームとビジネスの OneDrive の検索ビューの関連性の低い結果を表示するたとえば、します。</span><span class="sxs-lookup"><span data-stu-id="d4496-137">Setting to true also affects the relevance of the content displayed in Office 365 - for example, Suggested sites in SharePoint Home and the Discover view in OneDrive for Business show less relevant results.</span></span> <span data-ttu-id="d4496-138">この設定は、 [Office の説明](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout)でコントロールの状態を反映しています。</span><span class="sxs-lookup"><span data-stu-id="d4496-138">This setting reflects the control state in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span>|

## <a name="example"></a><span data-ttu-id="d4496-139">例</span><span class="sxs-lookup"><span data-stu-id="d4496-139">Example</span></span> 

##### <a name="request"></a><span data-ttu-id="d4496-140">要求</span><span class="sxs-lookup"><span data-stu-id="d4496-140">Request</span></span>

<span data-ttu-id="d4496-141">Delve のユーザーを無効にし、組織全体のコンテンツの関連性に関する彼の貢献度を無効にする方法について、例の要求は、ここで。</span><span class="sxs-lookup"><span data-stu-id="d4496-141">Here is an example request on how to opt-out a user from Delve and disable his contribution on content relevancy for the whole organization.</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/me/settings
Content-type: application/json
Content-length: 37

{
  "contributionToContentDiscoveryDisabled": true
}
```

##### <a name="response"></a><span data-ttu-id="d4496-142">応答</span><span class="sxs-lookup"><span data-stu-id="d4496-142">Response</span></span>

<span data-ttu-id="d4496-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d4496-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```

#### <a name="batch-request"></a><span data-ttu-id="d4496-146">バッチ要求</span><span class="sxs-lookup"><span data-stu-id="d4496-146">Batch request</span></span>

<span data-ttu-id="d4496-147">Delve から複数のユーザーを無効にし、バッチ要求を組織全体でのコンテンツの関連性のような貢献を無効にすることもできます。</span><span class="sxs-lookup"><span data-stu-id="d4496-147">It's also possible to opt-out multiple users from Delve and disable their contribution on content relevancy for the whole organization through a batch request.</span></span>
<span data-ttu-id="d4496-148">詳細については、 [JSON のバッチ処理](https://developer.microsoft.com/graph/docs/concepts/json_batching)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d4496-148">To learn more, see [JSON batching](https://developer.microsoft.com/graph/docs/concepts/json_batching).</span></span>

<span data-ttu-id="d4496-149">**重要**: だけで、[組織の管理](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US)役割グループのメンバーは、複数のユーザーを更新できます。</span><span class="sxs-lookup"><span data-stu-id="d4496-149">**Important**: Only members of the [Organization Management](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) role group can update multiple users.</span></span> 



