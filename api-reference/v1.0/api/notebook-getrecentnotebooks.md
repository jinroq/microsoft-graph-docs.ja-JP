---
title: 'ノートブック: getRecentNotebooks'
description: サインインしたユーザーによってアクセスされた recentNotebook インスタンスの一覧を取得します。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 1a629f405b2da1d395a927b12a1f5e1971c2e5f5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891235"
---
# <a name="notebook-getrecentnotebooks"></a><span data-ttu-id="07f47-103">ノートブック: getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="07f47-103">notebook: getRecentNotebooks</span></span>

<span data-ttu-id="07f47-104">サインインしたユーザーによってアクセスされた [recentNotebook](../resources/recentnotebook.md) インスタンスの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="07f47-104">Get a list of [recentNotebook](../resources/recentnotebook.md) instances that have been accessed by the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="07f47-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="07f47-105">Permissions</span></span>
<span data-ttu-id="07f47-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="07f47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07f47-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="07f47-108">Permission type</span></span>      | <span data-ttu-id="07f47-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="07f47-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07f47-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="07f47-110">Delegated (work or school account)</span></span> | <span data-ttu-id="07f47-111">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All、</span><span class="sxs-lookup"><span data-stu-id="07f47-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span></span>|
|<span data-ttu-id="07f47-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="07f47-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07f47-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07f47-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span> |
|<span data-ttu-id="07f47-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="07f47-114">Application</span></span> | <span data-ttu-id="07f47-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07f47-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="07f47-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="07f47-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
GET /users/{id | userPrincipalName}/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
```

<span data-ttu-id="07f47-117">ユーザーの `{id | userPrincipalName}` は、要求を行うために使用された承認トークンにおいてエンコードされたユーザーと一致しなければなりません。</span><span class="sxs-lookup"><span data-stu-id="07f47-117">The `{id | userPrincipalName}` for the user must match the user encoded in the authorization token used to make the request.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="07f47-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="07f47-118">Function parameters</span></span>

| <span data-ttu-id="07f47-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="07f47-119">Parameter</span></span>    | <span data-ttu-id="07f47-120">型</span><span class="sxs-lookup"><span data-stu-id="07f47-120">Type</span></span>   |<span data-ttu-id="07f47-121">説明</span><span class="sxs-lookup"><span data-stu-id="07f47-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07f47-122">includePersonalNotebooks</span><span class="sxs-lookup"><span data-stu-id="07f47-122">includePersonalNotebooks</span></span>|<span data-ttu-id="07f47-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="07f47-123">Boolean</span></span>|<span data-ttu-id="07f47-124">ユーザーが所有しているノートブックを含みます。</span><span class="sxs-lookup"><span data-stu-id="07f47-124">Include notebooks owned by the user.</span></span> <span data-ttu-id="07f47-125">ユーザーが所有しているノートブックを含むには、`true` に設定します。そうでない場合は、`false` に設定します。</span><span class="sxs-lookup"><span data-stu-id="07f47-125">Set to `true` to include notebooks owned by the user; otherwise, set to `false`.</span></span> <span data-ttu-id="07f47-126">`includePersonalNotebooks` パラメーターを含めない場合、要求は `400` エラー応答を返します。</span><span class="sxs-lookup"><span data-stu-id="07f47-126">If you don't include the `includePersonalNotebooks` parameter, your request will return a `400` error response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="07f47-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="07f47-127">Request headers</span></span>
| <span data-ttu-id="07f47-128">名前</span><span class="sxs-lookup"><span data-stu-id="07f47-128">Name</span></span>       | <span data-ttu-id="07f47-129">説明</span><span class="sxs-lookup"><span data-stu-id="07f47-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="07f47-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="07f47-130">Authorization</span></span>  | <span data-ttu-id="07f47-131">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="07f47-131">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="07f47-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="07f47-132">Request body</span></span>
<span data-ttu-id="07f47-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="07f47-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07f47-134">応答</span><span class="sxs-lookup"><span data-stu-id="07f47-134">Response</span></span>
<span data-ttu-id="07f47-135">正常な応答は **recentNotebooks** の JSON コレクションを含む `200 OK` を返します。</span><span class="sxs-lookup"><span data-stu-id="07f47-135">A successful response returns a `200 OK` that contains a JSON collection of **recentNotebooks**.</span></span>

## <a name="example"></a><span data-ttu-id="07f47-136">例</span><span class="sxs-lookup"><span data-stu-id="07f47-136">Example</span></span>
<span data-ttu-id="07f47-137">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="07f47-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="07f47-138">要求</span><span class="sxs-lookup"><span data-stu-id="07f47-138">Request</span></span>
<span data-ttu-id="07f47-139">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="07f47-139">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="07f47-140">プロトコル</span><span class="sxs-lookup"><span data-stu-id="07f47-140">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "recent_notebooks", "scopes": "notes.read" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=true)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="07f47-141">C#</span><span class="sxs-lookup"><span data-stu-id="07f47-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/recent-notebooks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="07f47-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="07f47-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/recent-notebooks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="07f47-143">目的-C</span><span class="sxs-lookup"><span data-stu-id="07f47-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/recent-notebooks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="07f47-144">Java</span><span class="sxs-lookup"><span data-stu-id="07f47-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/recent-notebooks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="07f47-145">応答</span><span class="sxs-lookup"><span data-stu-id="07f47-145">Response</span></span>
<span data-ttu-id="07f47-146">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="07f47-146">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.recentNotebook)",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 1110

{
  "value":[
    {
      "displayName":"Personal Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDrive"
    },{
      "displayName":"Team Shared Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDriveForBusiness"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
