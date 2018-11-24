# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a><span data-ttu-id="df33e-101">マイクロソフト チーム アプリケーション カタログから公開されているアプリケーションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="df33e-101">List the published apps from the Microsoft Teams app catalog</span></span>



<span data-ttu-id="df33e-102">マイクロソフト チーム アプリケーション カタログから[アプリケーション](../resources/teamsapp.md)を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="df33e-102">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span> <span data-ttu-id="df33e-103">これには、組織のアプリケーション カタログ (テナント アプリケーション カタログ) からアプリケーションと同様に、マイクロソフトのチーム ・ ストアからのアプリが含まれます。</span><span class="sxs-lookup"><span data-stu-id="df33e-103">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="df33e-104">組織のアプリケーションのカタログのみからアプリケーションを取得するのには次のように指定します。 `Organization` [teamsCatalogApp](../resources/teamsapp.md)リソースで**distributionMethod**とします。</span><span class="sxs-lookup"><span data-stu-id="df33e-104">To get apps from your organization's app catalog only, specify `Organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="df33e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="df33e-105">Permissions</span></span>

<span data-ttu-id="df33e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="df33e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="df33e-108">**注:** グローバル管理者だけでは、この API を呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="df33e-108">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="df33e-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="df33e-109">Permission Type</span></span>                        | <span data-ttu-id="df33e-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="df33e-110">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="df33e-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="df33e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="df33e-112">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df33e-112">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="df33e-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="df33e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df33e-114">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="df33e-114">Not supported</span></span>|
| <span data-ttu-id="df33e-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="df33e-115">Application</span></span>                            | <span data-ttu-id="df33e-116">非サポート</span><span class="sxs-lookup"><span data-stu-id="df33e-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="df33e-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="df33e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="df33e-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="df33e-118">Optional query parameters</span></span>
<span data-ttu-id="df33e-119">このメソッドは、$filter、$select をサポートしていて、$ は、応答をカスタマイズするために[OData クエリ パラメーター](../../../concepts/query_parameters.md)を展開します。</span><span class="sxs-lookup"><span data-stu-id="df33e-119">This method supports the $filter, $select, and $expand [OData query parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="df33e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="df33e-120">Request headers</span></span>

| <span data-ttu-id="df33e-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="df33e-121">Header</span></span>        | <span data-ttu-id="df33e-122">値</span><span class="sxs-lookup"><span data-stu-id="df33e-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="df33e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="df33e-123">Authorization</span></span> | <span data-ttu-id="df33e-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="df33e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="df33e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="df33e-126">Request body</span></span>
<span data-ttu-id="df33e-127">なし。</span><span class="sxs-lookup"><span data-stu-id="df33e-127">None.</span></span>

><span data-ttu-id="df33e-128">**注:** 任意の結果の一覧を短縮するための[teamsCatalogApp](../resources/teamsapp.md)オブジェクトのフィールドをフィルターできます。</span><span class="sxs-lookup"><span data-stu-id="df33e-128">**Note:** You can filter on any of the fields of the [teamsCatalogApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="df33e-129">次のフィルター操作のいずれかを使用することができます: 等しい、等しくない、またはではなく。</span><span class="sxs-lookup"><span data-stu-id="df33e-129">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="response"></a><span data-ttu-id="df33e-130">応答</span><span class="sxs-lookup"><span data-stu-id="df33e-130">Response</span></span>
<span data-ttu-id="df33e-131">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[teamsCatalogApp](../resources/teamsapp.md)オブジェクトの一覧です。</span><span class="sxs-lookup"><span data-stu-id="df33e-131">If successful, this method returns a `200 OK` response code and a list of [teamsCatalogApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="df33e-132">例</span><span class="sxs-lookup"><span data-stu-id="df33e-132">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="df33e-133">例 1</span><span class="sxs-lookup"><span data-stu-id="df33e-133">Example 1</span></span>
<span data-ttu-id="df33e-134">次の例では、テナントに固有のすべてのアプリケーションが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="df33e-134">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="df33e-135">要求</span><span class="sxs-lookup"><span data-stu-id="df33e-135">Request</span></span>
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

#### <a name="response"></a><span data-ttu-id="df33e-136">応答</span><span class="sxs-lookup"><span data-stu-id="df33e-136">Response</span></span>
```
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod":"Organization"
    }
  ]
}
```

### <a name="example-2"></a><span data-ttu-id="df33e-137">例 2</span><span class="sxs-lookup"><span data-stu-id="df33e-137">Example 2</span></span>

<span data-ttu-id="df33e-138">次の使用例は指定された ID を使用してアプリケーションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="df33e-138">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="df33e-139">要求</span><span class="sxs-lookup"><span data-stu-id="df33e-139">Request</span></span>
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="df33e-140">応答</span><span class="sxs-lookup"><span data-stu-id="df33e-140">Response</span></span>
```
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod":"Organization"
    }
  ]
}
```

