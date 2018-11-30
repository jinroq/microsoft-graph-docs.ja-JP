---
title: ボックスの一覧のリソース
description: この送信に関連付けられているリソースを一覧表示します。 **SubmissionResource**は、受講者の実際のリソース オブジェクトのラッパーは、作業です。 ラッパーには、割り当てのリソースへのポインターも含まれていますこれは、割り当て処理中に割り当てからコピーした場合。 これらのリソースは、割り当ての作業用コピーです。 **SubmittedResources**は、採点方式のことを正式に提出したリソースです。
ms.openlocfilehash: 0035f34b734cb4335fd1fd9ec3eece9183eed67b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067982"
---
# <a name="list-resources"></a><span data-ttu-id="7fdd2-107">ボックスの一覧のリソース</span><span class="sxs-lookup"><span data-stu-id="7fdd2-107">List resources</span></span>

> <span data-ttu-id="7fdd2-108">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7fdd2-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7fdd2-109">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7fdd2-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7fdd2-110">この送信に関連付けられているリソースを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="7fdd2-110">List the resources associated with this submission.</span></span> <span data-ttu-id="7fdd2-111">**SubmissionResource**は、受講者の実際のリソース オブジェクトのラッパーは、作業です。</span><span class="sxs-lookup"><span data-stu-id="7fdd2-111">The **submissionResource** object is a wrapper around the actual resource object the student is working on.</span></span> <span data-ttu-id="7fdd2-112">ラッパーには、割り当てのリソースへのポインターも含まれていますこれは、割り当て処理中に割り当てからコピーした場合。</span><span class="sxs-lookup"><span data-stu-id="7fdd2-112">The wrapper also includes a pointer to the resources on the assignment if this was copied from the assignment during the assign process.</span></span> <span data-ttu-id="7fdd2-113">これらのリソースは、割り当ての作業用コピーです。</span><span class="sxs-lookup"><span data-stu-id="7fdd2-113">These resources are the working copy of the assignment.</span></span> <span data-ttu-id="7fdd2-114">**SubmittedResources**は、採点方式のことを正式に提出したリソースです。</span><span class="sxs-lookup"><span data-stu-id="7fdd2-114">The **submittedResources** are the resources that have officially been submitted to be graded.</span></span>

## <a name="permissions"></a><span data-ttu-id="7fdd2-115">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7fdd2-115">Permissions</span></span>
<span data-ttu-id="7fdd2-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7fdd2-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fdd2-118">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7fdd2-118">Permission type</span></span>      | <span data-ttu-id="7fdd2-119">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7fdd2-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7fdd2-120">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7fdd2-120">Delegated (work or school account)</span></span> |  <span data-ttu-id="7fdd2-121">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7fdd2-121">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="7fdd2-122">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7fdd2-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fdd2-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7fdd2-123">Not supported.</span></span>   |
|<span data-ttu-id="7fdd2-124">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7fdd2-124">Application</span></span> | <span data-ttu-id="7fdd2-125">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7fdd2-125">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7fdd2-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7fdd2-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /educationClasses/assignments/{id}/submissions/{id}/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7fdd2-127">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7fdd2-127">Optional query parameters</span></span>
<span data-ttu-id="7fdd2-128">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7fdd2-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7fdd2-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7fdd2-129">Request headers</span></span>
| <span data-ttu-id="7fdd2-130">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7fdd2-130">Header</span></span>       | <span data-ttu-id="7fdd2-131">値</span><span class="sxs-lookup"><span data-stu-id="7fdd2-131">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7fdd2-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="7fdd2-132">Authorization</span></span>  | <span data-ttu-id="7fdd2-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7fdd2-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7fdd2-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="7fdd2-135">Request body</span></span>
<span data-ttu-id="7fdd2-136">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7fdd2-136">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7fdd2-137">応答</span><span class="sxs-lookup"><span data-stu-id="7fdd2-137">Response</span></span>
<span data-ttu-id="7fdd2-138">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[educationSubmissionResource](../resources/educationsubmissionresource.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="7fdd2-138">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7fdd2-139">例</span><span class="sxs-lookup"><span data-stu-id="7fdd2-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7fdd2-140">要求</span><span class="sxs-lookup"><span data-stu-id="7fdd2-140">Request</span></span>
<span data-ttu-id="7fdd2-141">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7fdd2-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_resources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/<id>/assignments/<id>/submissions/<id>/resources
```
##### <a name="response"></a><span data-ttu-id="7fdd2-142">応答</span><span class="sxs-lookup"><span data-stu-id="7fdd2-142">Response</span></span>
<span data-ttu-id="7fdd2-143">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7fdd2-143">The following is an example of the response.</span></span> 

><span data-ttu-id="7fdd2-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7fdd2-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List resources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->