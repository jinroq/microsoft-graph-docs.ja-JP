# <a name="group-checkmembergroups"></a><span data-ttu-id="71162-101">グループ: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="71162-101">group: checkMemberGroups</span></span>

<span data-ttu-id="71162-p101">指定したグループ一覧内のメンバーシップを確認します。指定したグループがダイレクト メンバーシップまたは推移性メンバーシップを持つグループを一覧から返します。</span><span class="sxs-lookup"><span data-stu-id="71162-p101">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="71162-p102">要求ごとに、最大 20 のグループを確認できます。この関数は、Office 365 と Azure AD でプロビジョニングされた他の種類のグループをサポートしています。Office 365 グループにはグループを含めることはできませんのでご注意ください。そのため、Office 365 グループのメンバーシップは常にダイレクト メンバーシップです。</span><span class="sxs-lookup"><span data-stu-id="71162-p102">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="71162-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="71162-108">Permissions</span></span>

<span data-ttu-id="71162-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="71162-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="71162-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="71162-111">Permission type</span></span>                        | <span data-ttu-id="71162-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="71162-112">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="71162-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="71162-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="71162-114">~~Group.Read.All~~、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="71162-114">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="71162-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="71162-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71162-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71162-116">Not supported.</span></span>                                                                              |
| <span data-ttu-id="71162-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="71162-117">Application</span></span>                            | <span data-ttu-id="71162-118">_Group.Read.All_、Directory.Read.All。</span><span class="sxs-lookup"><span data-stu-id="71162-118">_Group.Read.All_, Directory.Read.All, Directory.ReadWrite.All</span></span> <span data-ttu-id="71162-119">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71162-119">Directory.ReadWrite.All</span></span>                               |

> <span data-ttu-id="71162-120">**注:** この API では現在、`Directory.Read.All` 以上のアクセス権が必要です。</span><span class="sxs-lookup"><span data-stu-id="71162-120">Note: This API currently requires the Directory.Read.All permission or higher.</span></span> <span data-ttu-id="71162-121">`Group.Read.All` のアクセス許可を使用するとエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="71162-121">Using the Group.Read.All permission will return an error.</span></span> <span data-ttu-id="71162-122">これは既知のバグです。</span><span class="sxs-lookup"><span data-stu-id="71162-122">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="71162-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="71162-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="71162-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="71162-124">Request headers</span></span>

| <span data-ttu-id="71162-125">名前</span><span class="sxs-lookup"><span data-stu-id="71162-125">Name</span></span>          | <span data-ttu-id="71162-126">型</span><span class="sxs-lookup"><span data-stu-id="71162-126">Type</span></span>   | <span data-ttu-id="71162-127">説明</span><span class="sxs-lookup"><span data-stu-id="71162-127">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="71162-128">承認</span><span class="sxs-lookup"><span data-stu-id="71162-128">Authorization</span></span> | <span data-ttu-id="71162-129">文字列</span><span class="sxs-lookup"><span data-stu-id="71162-129">string</span></span> | <span data-ttu-id="71162-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="71162-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71162-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="71162-132">Request body</span></span>

<span data-ttu-id="71162-133">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="71162-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="71162-134">パラメーター</span><span class="sxs-lookup"><span data-stu-id="71162-134">Parameter</span></span> | <span data-ttu-id="71162-135">型</span><span class="sxs-lookup"><span data-stu-id="71162-135">Type</span></span>              | <span data-ttu-id="71162-136">説明</span><span class="sxs-lookup"><span data-stu-id="71162-136">Description</span></span>           |
| :-------- | :---------------- | :-------------------- |
| <span data-ttu-id="71162-137">groupIds</span><span class="sxs-lookup"><span data-stu-id="71162-137">groupIds</span></span>  | <span data-ttu-id="71162-138">String コレクション</span><span class="sxs-lookup"><span data-stu-id="71162-138">String collection</span></span> | <span data-ttu-id="71162-139">グループ ID の配列</span><span class="sxs-lookup"><span data-stu-id="71162-139">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="71162-140">応答</span><span class="sxs-lookup"><span data-stu-id="71162-140">Response</span></span>

<span data-ttu-id="71162-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="71162-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71162-142">例</span><span class="sxs-lookup"><span data-stu-id="71162-142">Example</span></span>

<span data-ttu-id="71162-143">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="71162-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="71162-144">要求</span><span class="sxs-lookup"><span data-stu-id="71162-144">Request</span></span>

<span data-ttu-id="71162-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="71162-145">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="71162-146">応答</span><span class="sxs-lookup"><span data-stu-id="71162-146">Response</span></span>

<span data-ttu-id="71162-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="71162-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
