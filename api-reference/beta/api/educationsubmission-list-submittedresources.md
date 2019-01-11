---
title: リスト submittedResources
description: グレーディングを正式に提出したリソースの一覧を表示します。 提出書類を所有している受講生受講者は、割り当てを再実行せず、提出済みのリストを変更できません。 これは実際のリソースのラッパーであり、このリソースは割り当てからコピーされた場合、実際の割り当てのリソースに戻るポインターを含めることができます。
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: da036713e6683aaef6576145dfe32b3b6eeaf11e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824144"
---
# <a name="list-submittedresources"></a><span data-ttu-id="2634d-105">リスト submittedResources</span><span class="sxs-lookup"><span data-stu-id="2634d-105">List submittedResources</span></span>

> <span data-ttu-id="2634d-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2634d-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2634d-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2634d-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2634d-108">グレーディングを正式に提出したリソースの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="2634d-108">List the resources that have officially been submitted for grading.</span></span> <span data-ttu-id="2634d-109">提出書類を所有している受講生受講者は、割り当てを再実行せず、提出済みのリストを変更できません。</span><span class="sxs-lookup"><span data-stu-id="2634d-109">The student who owns the submission cannot change the submitted list without resubmitting the assignment.</span></span> <span data-ttu-id="2634d-110">これは実際のリソースのラッパーであり、このリソースは割り当てからコピーされた場合、実際の割り当てのリソースに戻るポインターを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="2634d-110">This is a wrapper around the real resource and can contain a pointer back to the actual assignment resource if this resource was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="2634d-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2634d-111">Permissions</span></span>
<span data-ttu-id="2634d-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2634d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2634d-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2634d-114">Permission type</span></span>      | <span data-ttu-id="2634d-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2634d-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2634d-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2634d-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="2634d-117">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2634d-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="2634d-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2634d-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2634d-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2634d-119">Not supported.</span></span>  |
|<span data-ttu-id="2634d-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2634d-120">Application</span></span> | <span data-ttu-id="2634d-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2634d-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2634d-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2634d-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2634d-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2634d-123">Optional query parameters</span></span>
<span data-ttu-id="2634d-124">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2634d-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2634d-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2634d-125">Request headers</span></span>
| <span data-ttu-id="2634d-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2634d-126">Header</span></span>       | <span data-ttu-id="2634d-127">値</span><span class="sxs-lookup"><span data-stu-id="2634d-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2634d-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="2634d-128">Authorization</span></span>  | <span data-ttu-id="2634d-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2634d-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2634d-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="2634d-131">Request body</span></span>
<span data-ttu-id="2634d-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2634d-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2634d-133">応答</span><span class="sxs-lookup"><span data-stu-id="2634d-133">Response</span></span>
<span data-ttu-id="2634d-134">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[educationSubmissionResource](../resources/educationsubmissionresource.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="2634d-134">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2634d-135">例</span><span class="sxs-lookup"><span data-stu-id="2634d-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2634d-136">要求</span><span class="sxs-lookup"><span data-stu-id="2634d-136">Request</span></span>
<span data-ttu-id="2634d-137">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2634d-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submittedresources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submittedResources
```
##### <a name="response"></a><span data-ttu-id="2634d-138">応答</span><span class="sxs-lookup"><span data-stu-id="2634d-138">Response</span></span>
<span data-ttu-id="2634d-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2634d-139">The following is an example of the response.</span></span> 

><span data-ttu-id="2634d-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2634d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmittedSubmissionResource",
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
        "link": "https://www.microsoft.com
        },
        "@odata.type": "microsoft.graph.educationSubmittedSubmissionResource" 
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List submittedResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
