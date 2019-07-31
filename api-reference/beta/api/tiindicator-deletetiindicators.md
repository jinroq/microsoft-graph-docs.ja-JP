---
title: 'tiIndicator: deleteTiIndicators'
description: 複数の要求ではなく、1つの要求で複数の脅威インテリジェンス (TI) インジケーターを削除します。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 861b0ad0a476cfcc659bb20764b09d159c0ad61f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977490"
---
# <a name="tiindicator-deletetiindicators"></a><span data-ttu-id="c8972-103">tiIndicator: deleteTiIndicators</span><span class="sxs-lookup"><span data-stu-id="c8972-103">tiIndicator: deleteTiIndicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8972-104">複数の要求ではなく、1つの要求で複数の脅威インテリジェンス (TI) インジケーターを削除します。</span><span class="sxs-lookup"><span data-stu-id="c8972-104">Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8972-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c8972-105">Permissions</span></span>

<span data-ttu-id="c8972-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8972-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c8972-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c8972-108">Permission type</span></span> | <span data-ttu-id="c8972-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c8972-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c8972-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c8972-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c8972-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="c8972-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="c8972-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c8972-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8972-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8972-113">Not supported.</span></span> |
| <span data-ttu-id="c8972-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c8972-114">Application</span></span>                            | <span data-ttu-id="c8972-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="c8972-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8972-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c8972-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="c8972-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8972-117">Request headers</span></span>

| <span data-ttu-id="c8972-118">名前</span><span class="sxs-lookup"><span data-stu-id="c8972-118">Name</span></span>          | <span data-ttu-id="c8972-119">説明</span><span class="sxs-lookup"><span data-stu-id="c8972-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c8972-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8972-120">Authorization</span></span> | <span data-ttu-id="c8972-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c8972-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8972-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="c8972-122">Request body</span></span>

<span data-ttu-id="c8972-123">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="c8972-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c8972-124">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c8972-124">Parameter</span></span>    | <span data-ttu-id="c8972-125">型</span><span class="sxs-lookup"><span data-stu-id="c8972-125">Type</span></span>        | <span data-ttu-id="c8972-126">説明</span><span class="sxs-lookup"><span data-stu-id="c8972-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c8972-127">value</span><span class="sxs-lookup"><span data-stu-id="c8972-127">value</span></span>|<span data-ttu-id="c8972-128">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="c8972-128">String collection</span></span>| <span data-ttu-id="c8972-129">削除する tiIndicator `id`s のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="c8972-129">Collection of tiIndicator `id`s to be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="c8972-130">応答</span><span class="sxs-lookup"><span data-stu-id="c8972-130">Response</span></span>

<span data-ttu-id="c8972-131">成功した場合、この`200, OK`メソッドは応答コードと、応答本文で[resultinfo](../resources/resultinfo.md)コレクションオブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c8972-131">If successful, this method returns `200, OK` response code and a [resultInfo](../resources/resultinfo.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c8972-132">例</span><span class="sxs-lookup"><span data-stu-id="c8972-132">Examples</span></span>

<span data-ttu-id="c8972-133">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="c8972-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="c8972-134">要求</span><span class="sxs-lookup"><span data-stu-id="c8972-134">Request</span></span>

<span data-ttu-id="c8972-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c8972-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c8972-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c8972-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tiindicator_deletetiindicators"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicators
Content-type: application/json

{
  "value": [
    "id-value1",
    "id-value2"
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c8972-137">C#</span><span class="sxs-lookup"><span data-stu-id="c8972-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-deletetiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c8972-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="c8972-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-deletetiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c8972-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="c8972-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-deletetiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c8972-140">Java</span><span class="sxs-lookup"><span data-stu-id="c8972-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tiindicator-deletetiindicators-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c8972-141">応答</span><span class="sxs-lookup"><span data-stu-id="c8972-141">Response</span></span>

<span data-ttu-id="c8972-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c8972-142">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="c8972-143">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="c8972-143">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c8972-144">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c8972-144">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.resultInfo",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "code": "code-value",
      "message": "message-value",
      "subCode": "subCode-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: deleteTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
