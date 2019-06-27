---
title: 'ノートブック: getNotebookFromWebUrl'
description: URL パスを使用して、ノートブックオブジェクトのプロパティとリレーションシップを取得します。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: a27f787cdedf77f0ea4237067f537d6756bcc2bc
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266403"
---
# <a name="notebook-getnotebookfromweburl"></a><span data-ttu-id="a8574-103">ノートブック: getNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="a8574-103">notebook: getNotebookFromWebUrl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8574-104">URL パスを使用して、[ノートブック](../resources/notebook.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="a8574-104">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object by using its URL path.</span></span>

<span data-ttu-id="a8574-105">この場所は、office 365、グループノートブック、または Office 365 上の SharePoint サイトでホストされるチームノートブックのユーザーノートブックであることができます。</span><span class="sxs-lookup"><span data-stu-id="a8574-105">The location can be user notebooks on Office 365, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span>
## <a name="permissions"></a><span data-ttu-id="a8574-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a8574-106">Permissions</span></span>
<span data-ttu-id="a8574-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a8574-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8574-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a8574-109">Permission type</span></span>      | <span data-ttu-id="a8574-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a8574-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8574-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a8574-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a8574-112">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8574-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="a8574-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a8574-113">Application</span></span> | <span data-ttu-id="a8574-114">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8574-114">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8574-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a8574-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/GetNotebookFromWebUrl
POST /users/{id | userPrincipalName}/onenote/notebooks/GetNotebookFromWebUrl
POST /groups/{id}/onenote/notebooks/GetNotebookFromWebUrl
POST /sites/{id}/onenote/notebooks/GetNotebookFromWebUrl
```
## <a name="request-headers"></a><span data-ttu-id="a8574-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a8574-116">Request headers</span></span>
| <span data-ttu-id="a8574-117">名前</span><span class="sxs-lookup"><span data-stu-id="a8574-117">Name</span></span>       | <span data-ttu-id="a8574-118">型</span><span class="sxs-lookup"><span data-stu-id="a8574-118">Type</span></span> | <span data-ttu-id="a8574-119">説明</span><span class="sxs-lookup"><span data-stu-id="a8574-119">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a8574-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8574-120">Authorization</span></span>  | <span data-ttu-id="a8574-121">string</span><span class="sxs-lookup"><span data-stu-id="a8574-121">string</span></span>  | <span data-ttu-id="a8574-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a8574-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a8574-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a8574-124">Accept</span></span> | <span data-ttu-id="a8574-125">string</span><span class="sxs-lookup"><span data-stu-id="a8574-125">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="a8574-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a8574-126">Request body</span></span>
<span data-ttu-id="a8574-127">要求本文で、取得するノートブックへの完全な URL パスの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a8574-127">In the request body, supply a JSON representation of the full URL path to the notebook you want to retrieve.</span></span>

| <span data-ttu-id="a8574-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a8574-128">Property</span></span>     | <span data-ttu-id="a8574-129">型</span><span class="sxs-lookup"><span data-stu-id="a8574-129">Type</span></span>        | <span data-ttu-id="a8574-130">説明</span><span class="sxs-lookup"><span data-stu-id="a8574-130">Description</span></span> |
|:-------------|:------------|:------------|
| `webUrl`     |`String`     | <span data-ttu-id="a8574-131">取得するノートブックの URL パス。</span><span class="sxs-lookup"><span data-stu-id="a8574-131">The URL path of the notebook to retrieve.</span></span> <span data-ttu-id="a8574-132">また、"onenote:" というプレフィックスを含めることもできます。</span><span class="sxs-lookup"><span data-stu-id="a8574-132">It can also contain a "onenote:" prefix.</span></span>|

## <a name="response"></a><span data-ttu-id="a8574-133">応答</span><span class="sxs-lookup"><span data-stu-id="a8574-133">Response</span></span>

<span data-ttu-id="a8574-134">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[notebook](../resources/notebook.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a8574-134">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a8574-135">例</span><span class="sxs-lookup"><span data-stu-id="a8574-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a8574-136">要求</span><span class="sxs-lookup"><span data-stu-id="a8574-136">Request</span></span>
<span data-ttu-id="a8574-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a8574-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_fromweburl"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/GetNotebookFromWebUrl
Content-type: application/json

{"webUrl":"webUrl value"}
```
##### <a name="response"></a><span data-ttu-id="a8574-138">応答</span><span class="sxs-lookup"><span data-stu-id="a8574-138">Response</span></span>
<span data-ttu-id="a8574-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="a8574-139">Here is an example of the response.</span></span> 

><span data-ttu-id="a8574-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a8574-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json; odata.metadata=minimal
Content-Length: 544

{
    "isDefault": true,
    "userRole": "userRole-value",
    "isShared": true,
    "sectionsUrl": "sectionUrl-value",
    "sectionGroupsUrl": "sectionGroupUrl-value",
    "links": {
        "oneNoteClientUrl": {
            "href": "href-value"
        },
        "oneNoteWebUrl": {
            "href": "href-value"
        }
    },
    "id": "id-value",
    "self": "self-value",
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a8574-142">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="a8574-142">SDK sample code</span></span>
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a8574-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="a8574-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/notebook_fromweburl-Javascript-snippets.md)]

# <a name="ctabcs"></a>[<span data-ttu-id="a8574-144">C#</span><span class="sxs-lookup"><span data-stu-id="a8574-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/notebook_fromweburl-Cs-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a8574-145">目的-C</span><span class="sxs-lookup"><span data-stu-id="a8574-145">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/notebook_fromweburl-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/notebook-getnotebookfromweburl.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/notebook-getnotebookfromweburl.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/notebook-getnotebookfromweburl.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
