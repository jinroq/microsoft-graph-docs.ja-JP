---
title: ボックスの一覧のリソース
description: この送信に関連付けられているリソースを一覧表示します。 **SubmissionResource**は、受講者の実際のリソース オブジェクトのラッパーは、作業です。 ラッパーには、割り当てのリソースへのポインターも含まれていますこれは、割り当て処理中に割り当てからコピーした場合。 これらのリソースは、割り当ての作業用コピーです。 **SubmittedResources**は、採点方式のことを正式に提出したリソースです。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b9069cb6ec20f65b82cacca8f862a05ff0af7b5d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526187"
---
# <a name="list-resources"></a><span data-ttu-id="86908-107">ボックスの一覧のリソース</span><span class="sxs-lookup"><span data-stu-id="86908-107">List resources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86908-108">この送信に関連付けられているリソースを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="86908-108">List the resources associated with this submission.</span></span> <span data-ttu-id="86908-109">**SubmissionResource**は、受講者の実際のリソース オブジェクトのラッパーは、作業です。</span><span class="sxs-lookup"><span data-stu-id="86908-109">The **submissionResource** object is a wrapper around the actual resource object the student is working on.</span></span> <span data-ttu-id="86908-110">ラッパーには、割り当てのリソースへのポインターも含まれていますこれは、割り当て処理中に割り当てからコピーした場合。</span><span class="sxs-lookup"><span data-stu-id="86908-110">The wrapper also includes a pointer to the resources on the assignment if this was copied from the assignment during the assign process.</span></span> <span data-ttu-id="86908-111">これらのリソースは、割り当ての作業用コピーです。</span><span class="sxs-lookup"><span data-stu-id="86908-111">These resources are the working copy of the assignment.</span></span> <span data-ttu-id="86908-112">**SubmittedResources**は、採点方式のことを正式に提出したリソースです。</span><span class="sxs-lookup"><span data-stu-id="86908-112">The **submittedResources** are the resources that have officially been submitted to be graded.</span></span>

## <a name="permissions"></a><span data-ttu-id="86908-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="86908-113">Permissions</span></span>
<span data-ttu-id="86908-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="86908-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86908-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="86908-116">Permission type</span></span>      | <span data-ttu-id="86908-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="86908-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86908-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="86908-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="86908-119">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="86908-119">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="86908-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="86908-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86908-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86908-121">Not supported.</span></span>   |
|<span data-ttu-id="86908-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="86908-122">Application</span></span> | <span data-ttu-id="86908-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86908-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="86908-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="86908-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /educationClasses/assignments/{id}/submissions/{id}/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="86908-125">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="86908-125">Optional query parameters</span></span>
<span data-ttu-id="86908-126">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="86908-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="86908-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="86908-127">Request headers</span></span>
| <span data-ttu-id="86908-128">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="86908-128">Header</span></span>       | <span data-ttu-id="86908-129">値</span><span class="sxs-lookup"><span data-stu-id="86908-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="86908-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="86908-130">Authorization</span></span>  | <span data-ttu-id="86908-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="86908-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="86908-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="86908-133">Request body</span></span>
<span data-ttu-id="86908-134">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="86908-134">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="86908-135">応答</span><span class="sxs-lookup"><span data-stu-id="86908-135">Response</span></span>
<span data-ttu-id="86908-136">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[educationSubmissionResource](../resources/educationsubmissionresource.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="86908-136">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="86908-137">例</span><span class="sxs-lookup"><span data-stu-id="86908-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86908-138">要求</span><span class="sxs-lookup"><span data-stu-id="86908-138">Request</span></span>
<span data-ttu-id="86908-139">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="86908-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_resources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/<id>/assignments/<id>/submissions/<id>/resources
```
##### <a name="response"></a><span data-ttu-id="86908-140">応答</span><span class="sxs-lookup"><span data-stu-id="86908-140">Response</span></span>
<span data-ttu-id="86908-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="86908-141">The following is an example of the response.</span></span> 

><span data-ttu-id="86908-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="86908-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmissionResource",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1045

{
  "value": [
    {
      "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
      "id": "f2387c3b-ec39-4bf2-a399-d7242677f024",
      "resource": {
          "@odata.type": "#microsoft.graph.educationLinkResource",
          "displayName": "Microsoft Homepage",
          "createdDateTime": "2017-10-21T07:52:45.5675913Z",
          "createdBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "lastModifiedDateTime": "2017-10-21T07:52:45.5675913Z",
          "lastModifiedBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "link": "https://www.microsoft.com"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List resources",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-list-resources.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
