---
title: AdministrativeUnit の削除
description: AdministrativeUnit を削除します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6d23a1d9de8bb844fe3595a26cdf6869b4f2817e
ms.sourcegitcommit: 27e8ddb53b699f70b676c9648db8f06bb8d831a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/27/2019
ms.locfileid: "35917993"
---
# <a name="delete-administrativeunit"></a><span data-ttu-id="6f0e3-103">AdministrativeUnit の削除</span><span class="sxs-lookup"><span data-stu-id="6f0e3-103">Delete administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f0e3-104">[AdministrativeUnit](../resources/administrativeunit.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="6f0e3-104">Delete an [administrativeUnit](../resources/administrativeunit.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6f0e3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6f0e3-105">Permissions</span></span>
<span data-ttu-id="6f0e3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6f0e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6f0e3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6f0e3-108">Permission type</span></span>      | <span data-ttu-id="6f0e3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6f0e3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f0e3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6f0e3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6f0e3-111">AdministrativeUnit。すべての Directory.accessasuser.all について</span><span class="sxs-lookup"><span data-stu-id="6f0e3-111">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6f0e3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6f0e3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f0e3-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6f0e3-113">Not supported.</span></span>    |
|<span data-ttu-id="6f0e3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6f0e3-114">Application</span></span> | <span data-ttu-id="6f0e3-115">AdministrativeUnit</span><span class="sxs-lookup"><span data-stu-id="6f0e3-115">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f0e3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6f0e3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}

```
## <a name="request-headers"></a><span data-ttu-id="6f0e3-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6f0e3-117">Request headers</span></span>
| <span data-ttu-id="6f0e3-118">名前</span><span class="sxs-lookup"><span data-stu-id="6f0e3-118">Name</span></span>       | <span data-ttu-id="6f0e3-119">説明</span><span class="sxs-lookup"><span data-stu-id="6f0e3-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6f0e3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f0e3-120">Authorization</span></span>  | <span data-ttu-id="6f0e3-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6f0e3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f0e3-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="6f0e3-123">Request body</span></span>
<span data-ttu-id="6f0e3-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6f0e3-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f0e3-125">応答</span><span class="sxs-lookup"><span data-stu-id="6f0e3-125">Response</span></span>

<span data-ttu-id="6f0e3-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="6f0e3-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f0e3-128">例</span><span class="sxs-lookup"><span data-stu-id="6f0e3-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6f0e3-129">要求</span><span class="sxs-lookup"><span data-stu-id="6f0e3-129">Request</span></span>
<span data-ttu-id="6f0e3-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6f0e3-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6f0e3-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="6f0e3-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_administrativeunit"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6f0e3-132">C#</span><span class="sxs-lookup"><span data-stu-id="6f0e3-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6f0e3-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="6f0e3-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6f0e3-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="6f0e3-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6f0e3-135">Java</span><span class="sxs-lookup"><span data-stu-id="6f0e3-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6f0e3-136">応答</span><span class="sxs-lookup"><span data-stu-id="6f0e3-136">Response</span></span>
<span data-ttu-id="6f0e3-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6f0e3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
