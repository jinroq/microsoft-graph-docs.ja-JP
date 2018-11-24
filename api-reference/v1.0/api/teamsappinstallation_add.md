# <a name="add-app-to-team"></a><span data-ttu-id="b7f34-101">アプリケーションをチームに追加します。</span><span class="sxs-lookup"><span data-stu-id="b7f34-101">Add app to team</span></span>



<span data-ttu-id="b7f34-102">指定された[チーム](../resources/team.md)には、[アプリケーション](../resources/teamsapp.md)をインストールします。</span><span class="sxs-lookup"><span data-stu-id="b7f34-102">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b7f34-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b7f34-103">Permissions</span></span>
<span data-ttu-id="b7f34-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b7f34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b7f34-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b7f34-106">Permission type</span></span>      | <span data-ttu-id="b7f34-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b7f34-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7f34-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b7f34-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b7f34-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7f34-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b7f34-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b7f34-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7f34-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7f34-111">Not supported.</span></span>    |
|<span data-ttu-id="b7f34-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b7f34-112">Application</span></span> | <span data-ttu-id="b7f34-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7f34-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7f34-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b7f34-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="b7f34-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b7f34-115">Request headers</span></span>
| <span data-ttu-id="b7f34-116">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b7f34-116">Header</span></span>       | <span data-ttu-id="b7f34-117">値</span><span class="sxs-lookup"><span data-stu-id="b7f34-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b7f34-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7f34-118">Authorization</span></span>  | <span data-ttu-id="b7f34-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b7f34-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b7f34-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="b7f34-121">Request body</span></span>

| <span data-ttu-id="b7f34-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7f34-122">Property</span></span>     | <span data-ttu-id="b7f34-123">型</span><span class="sxs-lookup"><span data-stu-id="b7f34-123">Type</span></span>   |<span data-ttu-id="b7f34-124">説明</span><span class="sxs-lookup"><span data-stu-id="b7f34-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7f34-125">teamsApp</span><span class="sxs-lookup"><span data-stu-id="b7f34-125">teamsApp</span></span>| [<span data-ttu-id="b7f34-126">teamsApp</span><span class="sxs-lookup"><span data-stu-id="b7f34-126">teamsApp</span></span>](../resources/teamsapp.md) |<span data-ttu-id="b7f34-127">追加するアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="b7f34-127">The app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="b7f34-128">応答</span><span class="sxs-lookup"><span data-stu-id="b7f34-128">Response</span></span>

<span data-ttu-id="b7f34-129">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="b7f34-129">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b7f34-130">例</span><span class="sxs-lookup"><span data-stu-id="b7f34-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b7f34-131">要求</span><span class="sxs-lookup"><span data-stu-id="b7f34-131">Request</span></span>
<span data-ttu-id="b7f34-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b7f34-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/installedApps
{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
#### <a name="response"></a><span data-ttu-id="b7f34-133">応答</span><span class="sxs-lookup"><span data-stu-id="b7f34-133">Response</span></span>
<span data-ttu-id="b7f34-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b7f34-134">The following is an example of the response.</span></span> <span data-ttu-id="b7f34-135">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="b7f34-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b7f34-136">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b7f34-136">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="b7f34-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="b7f34-137">See also</span></span>

