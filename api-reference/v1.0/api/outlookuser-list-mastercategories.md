---
title: Outlook カテゴリを一覧表示する
description: ユーザーに対して定義されているすべてのカテゴリを取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7423c81f5fbdf8f7f6181ba6079b39b500d6229a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36309463"
---
# <a name="list-outlook-categories"></a><span data-ttu-id="f8fbc-103">Outlook カテゴリを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f8fbc-103">List Outlook categories</span></span>


<span data-ttu-id="f8fbc-104">ユーザーに対して定義されているすべてのカテゴリを取得します。</span><span class="sxs-lookup"><span data-stu-id="f8fbc-104">Get all the categories that have been defined for the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8fbc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f8fbc-105">Permissions</span></span>
<span data-ttu-id="f8fbc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f8fbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8fbc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f8fbc-108">Permission type</span></span>      | <span data-ttu-id="f8fbc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f8fbc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8fbc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f8fbc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f8fbc-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="f8fbc-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="f8fbc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f8fbc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8fbc-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="f8fbc-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="f8fbc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f8fbc-114">Application</span></span> | <span data-ttu-id="f8fbc-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="f8fbc-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8fbc-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f8fbc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories
GET /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f8fbc-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f8fbc-117">Optional query parameters</span></span>
<span data-ttu-id="f8fbc-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f8fbc-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f8fbc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f8fbc-119">Request headers</span></span>
| <span data-ttu-id="f8fbc-120">名前</span><span class="sxs-lookup"><span data-stu-id="f8fbc-120">Name</span></span>      |<span data-ttu-id="f8fbc-121">説明</span><span class="sxs-lookup"><span data-stu-id="f8fbc-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f8fbc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8fbc-122">Authorization</span></span>  | <span data-ttu-id="f8fbc-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f8fbc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8fbc-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f8fbc-125">Request body</span></span>
<span data-ttu-id="f8fbc-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f8fbc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8fbc-127">応答</span><span class="sxs-lookup"><span data-stu-id="f8fbc-127">Response</span></span>

<span data-ttu-id="f8fbc-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文に [outlookCategory](../resources/outlookcategory.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f8fbc-128">If successful, this method returns a `200 OK` response code and collection of [outlookCategory](../resources/outlookcategory.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f8fbc-129">例</span><span class="sxs-lookup"><span data-stu-id="f8fbc-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f8fbc-130">要求</span><span class="sxs-lookup"><span data-stu-id="f8fbc-130">Request</span></span>
<span data-ttu-id="f8fbc-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f8fbc-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f8fbc-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="f8fbc-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mastercategories"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/outlook/masterCategories
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f8fbc-133">C#</span><span class="sxs-lookup"><span data-stu-id="f8fbc-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mastercategories-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f8fbc-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8fbc-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mastercategories-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f8fbc-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="f8fbc-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mastercategories-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f8fbc-136">Java</span><span class="sxs-lookup"><span data-stu-id="f8fbc-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mastercategories-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f8fbc-137">応答</span><span class="sxs-lookup"><span data-stu-id="f8fbc-137">Response</span></span>
<span data-ttu-id="f8fbc-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f8fbc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 727

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories",
  "value":[
    {
      "id":"5a9a6aa8-b65f-4357-b1f9-60c6bf6330d8",
      "displayName":"Red category",
      "color":"preset0"
    },
    {
      "id":"4b1c2495-54c9-4a5e-90a2-0ab0b31987d8",
      "displayName":"Orange category",
      "color":"preset1"
    },
    {
      "id":"de912e4d-c790-4da9-949c-ccd933aaa0f7",
      "displayName":"Yellow category",
      "color":"preset3"
    },
    {
      "id":"79c8d8f8-9db1-49ec-99ce-ae25793e7232",
      "displayName":"Green category",
      "color":"preset4"
    },
    {
      "id":"626e696c-6a10-48b8-89b9-12de3160cfb9",
      "displayName":"Blue category",
      "color":"preset7"
    },
    {
      "id":"453d06d0-447d-41f7-91cd-aa0f6b190b5b",
      "displayName":"Purple category",
      "color":"preset8"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List categories",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
