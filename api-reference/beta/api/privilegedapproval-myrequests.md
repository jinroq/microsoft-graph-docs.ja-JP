---
title: 'privilegedApproval: myRequests'
description: リクエスターの承認要求を取得します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 256eafec031c98ee2f850f2deb958f5db1a9fd6d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36361262"
---
# <a name="privilegedapproval-myrequests"></a><span data-ttu-id="040e3-103">privilegedApproval: myRequests</span><span class="sxs-lookup"><span data-stu-id="040e3-103">privilegedApproval: myRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="040e3-104">リクエスターの承認要求を取得します。</span><span class="sxs-lookup"><span data-stu-id="040e3-104">Get the requestor's approval requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="040e3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="040e3-105">Permissions</span></span>
<span data-ttu-id="040e3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="040e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="040e3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="040e3-108">Permission type</span></span>      | <span data-ttu-id="040e3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="040e3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="040e3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="040e3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="040e3-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="040e3-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="040e3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="040e3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="040e3-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="040e3-113">Not supported.</span></span>    |
|<span data-ttu-id="040e3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="040e3-114">Application</span></span> | <span data-ttu-id="040e3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="040e3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="040e3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="040e3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/myRequests

```
## <a name="request-headers"></a><span data-ttu-id="040e3-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="040e3-117">Request headers</span></span>
| <span data-ttu-id="040e3-118">名前</span><span class="sxs-lookup"><span data-stu-id="040e3-118">Name</span></span>       | <span data-ttu-id="040e3-119">説明</span><span class="sxs-lookup"><span data-stu-id="040e3-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="040e3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="040e3-120">Authorization</span></span>  | <span data-ttu-id="040e3-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="040e3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="040e3-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="040e3-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="040e3-124">応答</span><span class="sxs-lookup"><span data-stu-id="040e3-124">Response</span></span>

<span data-ttu-id="040e3-125">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[privilegedApproval](../resources/privilegedapproval.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="040e3-125">If successful, this method returns `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="040e3-126">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="040e3-126">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="040e3-127">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="040e3-127">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="040e3-128">例</span><span class="sxs-lookup"><span data-stu-id="040e3-128">Example</span></span>
<span data-ttu-id="040e3-129">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="040e3-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="040e3-130">要求</span><span class="sxs-lookup"><span data-stu-id="040e3-130">Request</span></span>
<span data-ttu-id="040e3-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="040e3-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="040e3-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="040e3-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedapproval_myrequests"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval/myRequests
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="040e3-133">C#</span><span class="sxs-lookup"><span data-stu-id="040e3-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedapproval-myrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="040e3-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="040e3-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedapproval-myrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="040e3-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="040e3-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedapproval-myrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="040e3-136">Java</span><span class="sxs-lookup"><span data-stu-id="040e3-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedapproval-myrequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="040e3-137">応答</span><span class="sxs-lookup"><span data-stu-id="040e3-137">Response</span></span>
<span data-ttu-id="040e3-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="040e3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 193

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedApproval: myRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
