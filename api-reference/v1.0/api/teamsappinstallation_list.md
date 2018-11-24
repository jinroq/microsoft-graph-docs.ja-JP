# <a name="list-apps-in-team"></a><span data-ttu-id="6e81d-101">チームでのアプリケーションの一覧</span><span class="sxs-lookup"><span data-stu-id="6e81d-101">List apps in team</span></span>



<span data-ttu-id="6e81d-102">[アプリケーションのインストール](../resources/teamsappinstallation.md)を指定された[チーム](../resources/team.md)での一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="6e81d-102">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6e81d-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6e81d-103">Permissions</span></span>

<span data-ttu-id="6e81d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6e81d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6e81d-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6e81d-106">Permission type</span></span>      | <span data-ttu-id="6e81d-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6e81d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e81d-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6e81d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6e81d-109">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e81d-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6e81d-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6e81d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e81d-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6e81d-111">Not supported.</span></span>    |
|<span data-ttu-id="6e81d-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6e81d-112">Application</span></span> | <span data-ttu-id="6e81d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6e81d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e81d-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6e81d-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6e81d-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6e81d-115">Optional query parameters</span></span>

<span data-ttu-id="6e81d-116">このメソッドは、$filter、$select をサポートしていて、$ は、応答をカスタマイズするために[OData クエリ パラメーター](../../../concepts/query_parameters.md)を展開します。</span><span class="sxs-lookup"><span data-stu-id="6e81d-116">This method supports the $filter, $select, and $expand [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e81d-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6e81d-117">Request headers</span></span>

| <span data-ttu-id="6e81d-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6e81d-118">Header</span></span>       | <span data-ttu-id="6e81d-119">値</span><span class="sxs-lookup"><span data-stu-id="6e81d-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6e81d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e81d-120">Authorization</span></span>  | <span data-ttu-id="6e81d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6e81d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6e81d-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="6e81d-123">Request body</span></span>

<span data-ttu-id="6e81d-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6e81d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e81d-125">応答</span><span class="sxs-lookup"><span data-stu-id="6e81d-125">Response</span></span>

<span data-ttu-id="6e81d-126">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[teamsApp](../resources/teamsapp.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="6e81d-126">If successful, this method returns a `200 OK` response code and collection of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e81d-127">例</span><span class="sxs-lookup"><span data-stu-id="6e81d-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e81d-128">要求</span><span class="sxs-lookup"><span data-stu-id="6e81d-128">Request</span></span>

<span data-ttu-id="6e81d-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6e81d-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps
```

### <a name="response"></a><span data-ttu-id="6e81d-130">応答</span><span class="sxs-lookup"><span data-stu-id="6e81d-130">Response</span></span>

<span data-ttu-id="6e81d-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6e81d-131">The following is an example of the response.</span></span>
><span data-ttu-id="6e81d-132">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="6e81d-132">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6e81d-133">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6e81d-133">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

## <a name="example----getting-the-names-of-the-installed-apps"></a><span data-ttu-id="6e81d-134">例--は、インストールされているアプリケーションの名前を取得します。</span><span class="sxs-lookup"><span data-stu-id="6e81d-134">Example -- getting the names of the installed apps</span></span>

### <a name="request"></a><span data-ttu-id="6e81d-135">要求</span><span class="sxs-lookup"><span data-stu-id="6e81d-135">Request</span></span>

<span data-ttu-id="6e81d-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6e81d-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps?$expand=teamsAppDefinition
```

### <a name="response"></a><span data-ttu-id="6e81d-137">応答</span><span class="sxs-lookup"><span data-stu-id="6e81d-137">Response</span></span>

<span data-ttu-id="6e81d-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6e81d-138">The following is an example of the response.</span></span>

><span data-ttu-id="6e81d-139">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="6e81d-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6e81d-140">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6e81d-140">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
    "value": [
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=",
            "teamsAppDefinition": {
                "id": "MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==",
                "teamsAppId": "0d820ecd-def2-4297-adad-78056cde7c78",
                "displayName": "OneNote",
                "version": "1.0.0"
            }
        },
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZmQ5MjVhMC0zNTdmLTRkMjUtODQ1Ni1iMzAyMmFhYTQxYTk=",
            "teamsAppDefinition": {
                "id": "MGZkOTI1YTAtMzU3Zi00ZDI1LTg0NTYtYjMwMjJhYWE0MWE5IyMxLjc=",
                "teamsAppId": "0fd925a0-357f-4d25-8456-b3022aaa41a9",
                "displayName": "SurveyMonkey",
                "version": "1.7"
            }
        },
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMyYTUyNzcwMy0xZjZmLTQ1NTktYTMzMi1kOGE3ZDI4OGNkODg=",
            "teamsAppDefinition": {
                "id": "MmE1Mjc3MDMtMWY2Zi00NTU5LWEzMzItZDhhN2QyODhjZDg4IyMxLjA=",
                "teamsAppId": "2a527703-1f6f-4559-a332-d8a7d288cd88",
                "displayName": "SharePoint",
                "version": "1.0"
            }
        }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->