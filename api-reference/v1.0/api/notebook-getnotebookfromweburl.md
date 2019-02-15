---
title: 'ノートブック: getNotebookFromWebUrl'
description: プロパティと URL パスを使用してノートブックのオブジェクトの関係を取得します。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 3d14edf5a8992f9f4386e4b50aa74d54986b62f1
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/13/2019
ms.locfileid: "29982063"
---
# <a name="notebook-getnotebookfromweburl"></a><span data-ttu-id="7a1b5-103">ノートブック: getNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="7a1b5-103">notebook: getNotebookFromWebUrl</span></span>

<span data-ttu-id="7a1b5-104">URL パスを使用して、プロパティと、[ノートブック](../resources/notebook.md)のオブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="7a1b5-104">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object by using its URL path.</span></span>

<span data-ttu-id="7a1b5-105">場所は、Office 365、グループのノート、または Office 365 で SharePoint サイトでホストされているチームのノート パソコンのユーザーのノートブックを指定できます。</span><span class="sxs-lookup"><span data-stu-id="7a1b5-105">The location can be user notebooks on Office 365, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span>
## <a name="permissions"></a><span data-ttu-id="7a1b5-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7a1b5-106">Permissions</span></span>
<span data-ttu-id="7a1b5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7a1b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a1b5-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7a1b5-109">Permission type</span></span>      | <span data-ttu-id="7a1b5-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7a1b5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a1b5-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7a1b5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7a1b5-112">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a1b5-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="7a1b5-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7a1b5-113">Application</span></span> | <span data-ttu-id="7a1b5-114">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a1b5-114">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a1b5-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7a1b5-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/GetNotebookFromWebUrl
POST /users/{id | userPrincipalName}/onenote/notebooks/GetNotebookFromWebUrl
POST /groups/{id}/onenote/notebooks/GetNotebookFromWebUrl
POST /sites/{id}/onenote/notebooks/GetNotebookFromWebUrl
```
## <a name="request-headers"></a><span data-ttu-id="7a1b5-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7a1b5-116">Request headers</span></span>
| <span data-ttu-id="7a1b5-117">名前</span><span class="sxs-lookup"><span data-stu-id="7a1b5-117">Name</span></span>       | <span data-ttu-id="7a1b5-118">型</span><span class="sxs-lookup"><span data-stu-id="7a1b5-118">Type</span></span> | <span data-ttu-id="7a1b5-119">説明</span><span class="sxs-lookup"><span data-stu-id="7a1b5-119">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7a1b5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a1b5-120">Authorization</span></span>  | <span data-ttu-id="7a1b5-121">string</span><span class="sxs-lookup"><span data-stu-id="7a1b5-121">string</span></span>  | <span data-ttu-id="7a1b5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7a1b5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7a1b5-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7a1b5-124">Accept</span></span> | <span data-ttu-id="7a1b5-125">string</span><span class="sxs-lookup"><span data-stu-id="7a1b5-125">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="7a1b5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7a1b5-126">Request body</span></span>
<span data-ttu-id="7a1b5-127">要求の本文には、ノートブックを取得する完全な URL パスの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="7a1b5-127">In the request body, supply a JSON representation of the full URL path to the notebook you want to retrieve.</span></span>

| <span data-ttu-id="7a1b5-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a1b5-128">Property</span></span>     | <span data-ttu-id="7a1b5-129">型</span><span class="sxs-lookup"><span data-stu-id="7a1b5-129">Type</span></span>        | <span data-ttu-id="7a1b5-130">説明</span><span class="sxs-lookup"><span data-stu-id="7a1b5-130">Description</span></span> |
|:-------------|:------------|:------------|
| `webUrl`     |`String`     | <span data-ttu-id="7a1b5-131">取得するためにノートブックの URL パスです。</span><span class="sxs-lookup"><span data-stu-id="7a1b5-131">The URL path of the notebook to retrieve.</span></span> <span data-ttu-id="7a1b5-132">含めることも、"onenote:"プレフィックス。</span><span class="sxs-lookup"><span data-stu-id="7a1b5-132">It can also contain a "onenote:" prefix.</span></span>|

## <a name="response"></a><span data-ttu-id="7a1b5-133">応答</span><span class="sxs-lookup"><span data-stu-id="7a1b5-133">Response</span></span>

<span data-ttu-id="7a1b5-134">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [notebook](../resources/notebook.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7a1b5-134">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7a1b5-135">例</span><span class="sxs-lookup"><span data-stu-id="7a1b5-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7a1b5-136">要求</span><span class="sxs-lookup"><span data-stu-id="7a1b5-136">Request</span></span>
<span data-ttu-id="7a1b5-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7a1b5-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_fromweburl"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/GetNotebookFromWebUrl
Content-type: application/json

{"webUrl":"webUrl value"}
```
##### <a name="response"></a><span data-ttu-id="7a1b5-138">応答</span><span class="sxs-lookup"><span data-stu-id="7a1b5-138">Response</span></span>
<span data-ttu-id="7a1b5-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="7a1b5-139">Here is an example of the response.</span></span> 

><span data-ttu-id="7a1b5-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7a1b5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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