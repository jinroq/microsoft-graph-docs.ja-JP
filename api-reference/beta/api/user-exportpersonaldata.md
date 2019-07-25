---
title: 'ユーザー: Exportpersonal Data'
description: 組織のユーザーのデータをエクスポートするために、会社の管理者によって行われたデータポリシー操作要求を送信します。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 50e0753ab717208bd5d4d6ec4cdd402a9487d321
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867780"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="1d2d3-103">ユーザー: Exportpersonal Data</span><span class="sxs-lookup"><span data-stu-id="1d2d3-103">user: exportPersonalData</span></span>

<span data-ttu-id="1d2d3-104">組織のユーザーのデータをエクスポートするために、会社の管理者によって行われたデータポリシー操作要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="1d2d3-104">Submits a data policy operation request, made by a company administrator to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d2d3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1d2d3-105">Permissions</span></span>
<span data-ttu-id="1d2d3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1d2d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d2d3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1d2d3-108">Permission type</span></span>      | <span data-ttu-id="1d2d3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1d2d3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d2d3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1d2d3-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="1d2d3-111">すべてのユーザーとユーザーの. すべてをエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="1d2d3-111">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="1d2d3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1d2d3-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1d2d3-113">該当なし</span><span class="sxs-lookup"><span data-stu-id="1d2d3-113">Not applicable</span></span>  |
|<span data-ttu-id="1d2d3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1d2d3-114">Application</span></span> | <span data-ttu-id="1d2d3-115">すべてのユーザーとユーザーの. すべてをエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="1d2d3-115">User.Export.All and User.Read.All</span></span> |

><span data-ttu-id="1d2d3-116">**注:** エクスポートは、委任されたアクセス許可を使用する場合にのみ、会社の管理者が実行できます。</span><span class="sxs-lookup"><span data-stu-id="1d2d3-116">**Note:** Export can only be performed by a company administrator when the delegated permission is used.</span></span>

## <a name="http-request"></a><span data-ttu-id="1d2d3-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1d2d3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/<id>/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="1d2d3-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d2d3-118">Request headers</span></span>
| <span data-ttu-id="1d2d3-119">名前</span><span class="sxs-lookup"><span data-stu-id="1d2d3-119">Name</span></span>       | <span data-ttu-id="1d2d3-120">説明</span><span class="sxs-lookup"><span data-stu-id="1d2d3-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="1d2d3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d2d3-121">Authorization</span></span>  | <span data-ttu-id="1d2d3-122">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="1d2d3-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d2d3-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="1d2d3-123">Request body</span></span>
<span data-ttu-id="1d2d3-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="1d2d3-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1d2d3-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="1d2d3-125">Parameter</span></span>    | <span data-ttu-id="1d2d3-126">型</span><span class="sxs-lookup"><span data-stu-id="1d2d3-126">Type</span></span>   |<span data-ttu-id="1d2d3-127">説明</span><span class="sxs-lookup"><span data-stu-id="1d2d3-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1d2d3-128">storageLocation</span><span class="sxs-lookup"><span data-stu-id="1d2d3-128">storageLocation</span></span>|<span data-ttu-id="1d2d3-129">String</span><span class="sxs-lookup"><span data-stu-id="1d2d3-129">String</span></span>|<span data-ttu-id="1d2d3-130">これは、データのエクスポート先となる Azure Storage アカウントの shared access signature (SAS) URL です。</span><span class="sxs-lookup"><span data-stu-id="1d2d3-130">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="1d2d3-131">応答</span><span class="sxs-lookup"><span data-stu-id="1d2d3-131">Response</span></span>
<span data-ttu-id="1d2d3-132">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="1d2d3-132">If successful, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="1d2d3-133">応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1d2d3-133">It does not return anything in the response body.</span></span> <span data-ttu-id="1d2d3-134">応答には、次のヘッダーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1d2d3-134">The response contains the following headers.</span></span>

| <span data-ttu-id="1d2d3-135">名前</span><span class="sxs-lookup"><span data-stu-id="1d2d3-135">Name</span></span>       | <span data-ttu-id="1d2d3-136">説明</span><span class="sxs-lookup"><span data-stu-id="1d2d3-136">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="1d2d3-137">Location</span><span class="sxs-lookup"><span data-stu-id="1d2d3-137">Location</span></span>  | <span data-ttu-id="1d2d3-138">要求の状態を確認するための URL。</span><span class="sxs-lookup"><span data-stu-id="1d2d3-138">URL to check on the status of the Request.</span></span> |
| <span data-ttu-id="1d2d3-139">再試行-後</span><span class="sxs-lookup"><span data-stu-id="1d2d3-139">Retry-After</span></span>  | <span data-ttu-id="1d2d3-140">期間 (秒単位)。</span><span class="sxs-lookup"><span data-stu-id="1d2d3-140">Time period in seconds.</span></span> <span data-ttu-id="1d2d3-141">要求を送信した後に、要求の状態を確認するための要求を送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1d2d3-141">Request maker should wait this long after submitting a request to check for the status.</span></span> |


## <a name="example"></a><span data-ttu-id="1d2d3-142">例</span><span class="sxs-lookup"><span data-stu-id="1d2d3-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1d2d3-143">要求</span><span class="sxs-lookup"><span data-stu-id="1d2d3-143">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1d2d3-144">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1d2d3-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_exportpersonaldata"
}-->
```http
POST https://graph.microsoft.com/beta/users/{id}/exportPersonalData
Content-type: application/json
Content-length: 48

{
  "storageLocation": "storageLocation-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1d2d3-145">C#</span><span class="sxs-lookup"><span data-stu-id="1d2d3-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-exportpersonaldata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1d2d3-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="1d2d3-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-exportpersonaldata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1d2d3-147">目的-C</span><span class="sxs-lookup"><span data-stu-id="1d2d3-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-exportpersonaldata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1d2d3-148">Java</span><span class="sxs-lookup"><span data-stu-id="1d2d3-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-exportpersonaldata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1d2d3-149">応答</span><span class="sxs-lookup"><span data-stu-id="1d2d3-149">Response</span></span>

```http
{
  Location: https://graph.microsoft.com/beta/dataPolicyOperations/d007e3da-cd9b-4b02-8d66-422403c53e3f
  Retry-After: 60
}
```

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: exportPersonalData",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
