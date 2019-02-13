---
title: 'ノートブック: getNotebookFromWebUrl'
description: プロパティと URL パスを使用してノートブックのオブジェクトの関係を取得します。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 226cbd70343feaf8fe5404aac6077f9b2438aba8
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/13/2019
ms.locfileid: "29982070"
---
# <a name="notebook-getnotebookfromweburl"></a><span data-ttu-id="65e96-103">ノートブック: getNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="65e96-103">notebook: getNotebookFromWebUrl</span></span>

[!ベータ版についての免責事項を含める]

<span data-ttu-id="65e96-105">URL パスを使用して、プロパティと、[ノートブック](../resources/notebook.md)のオブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="65e96-105">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object by using its URL path.</span></span>

<span data-ttu-id="65e96-106">場所は、Office 365、グループのノート、または Office 365 で SharePoint サイトでホストされているチームのノート パソコンのユーザーのノートブックを指定できます。</span><span class="sxs-lookup"><span data-stu-id="65e96-106">The location can be user notebooks on Office 365, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span>
## <a name="permissions"></a><span data-ttu-id="65e96-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="65e96-107">Permissions</span></span>
<span data-ttu-id="65e96-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65e96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65e96-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="65e96-110">Permission type</span></span>      | <span data-ttu-id="65e96-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="65e96-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65e96-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="65e96-112">Delegated (work or school account)</span></span> | <span data-ttu-id="65e96-113">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65e96-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="65e96-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="65e96-114">Application</span></span> | <span data-ttu-id="65e96-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65e96-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="65e96-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="65e96-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/GetNotebookFromWebUrl
POST /users/{id | userPrincipalName}/onenote/notebooks/GetNotebookFromWebUrl
POST /groups/{id}/onenote/notebooks/GetNotebookFromWebUrl
POST /sites/{id}/onenote/notebooks/GetNotebookFromWebUrl
```
## <a name="request-headers"></a><span data-ttu-id="65e96-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="65e96-117">Request headers</span></span>
| <span data-ttu-id="65e96-118">名前</span><span class="sxs-lookup"><span data-stu-id="65e96-118">Name</span></span>       | <span data-ttu-id="65e96-119">型</span><span class="sxs-lookup"><span data-stu-id="65e96-119">Type</span></span> | <span data-ttu-id="65e96-120">説明</span><span class="sxs-lookup"><span data-stu-id="65e96-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="65e96-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="65e96-121">Authorization</span></span>  | <span data-ttu-id="65e96-122">string</span><span class="sxs-lookup"><span data-stu-id="65e96-122">string</span></span>  | <span data-ttu-id="65e96-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="65e96-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="65e96-125">承諾</span><span class="sxs-lookup"><span data-stu-id="65e96-125">Accept</span></span> | <span data-ttu-id="65e96-126">string</span><span class="sxs-lookup"><span data-stu-id="65e96-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="65e96-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="65e96-127">Request body</span></span>
<span data-ttu-id="65e96-128">要求の本文には、ノートブックを取得する完全な URL パスの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="65e96-128">In the request body, supply a JSON representation of the full URL path to the notebook you want to retrieve.</span></span>

| <span data-ttu-id="65e96-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65e96-129">Property</span></span>     | <span data-ttu-id="65e96-130">型</span><span class="sxs-lookup"><span data-stu-id="65e96-130">Type</span></span>        | <span data-ttu-id="65e96-131">説明</span><span class="sxs-lookup"><span data-stu-id="65e96-131">Description</span></span> |
|:-------------|:------------|:------------|
| `webUrl`     |`String`     | <span data-ttu-id="65e96-132">取得するためにノートブックの URL パスです。</span><span class="sxs-lookup"><span data-stu-id="65e96-132">The URL path of the notebook to retrieve.</span></span> <span data-ttu-id="65e96-133">含めることも、"onenote:"プレフィックス。</span><span class="sxs-lookup"><span data-stu-id="65e96-133">It can also contain a "onenote:" prefix.</span></span>|

## <a name="response"></a><span data-ttu-id="65e96-134">応答</span><span class="sxs-lookup"><span data-stu-id="65e96-134">Response</span></span>

<span data-ttu-id="65e96-135">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [notebook](../resources/notebook.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="65e96-135">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="65e96-136">例</span><span class="sxs-lookup"><span data-stu-id="65e96-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="65e96-137">要求</span><span class="sxs-lookup"><span data-stu-id="65e96-137">Request</span></span>
<span data-ttu-id="65e96-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="65e96-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_fromweburl"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/GetNotebookFromWebUrl
Content-type: application/json

{"webUrl":"webUrl value"}
```
##### <a name="response"></a><span data-ttu-id="65e96-139">応答</span><span class="sxs-lookup"><span data-stu-id="65e96-139">Response</span></span>
<span data-ttu-id="65e96-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="65e96-140">Here is an example of the response.</span></span> 

><span data-ttu-id="65e96-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="65e96-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error:{notebook-getnotebookfromweburl.md}:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
