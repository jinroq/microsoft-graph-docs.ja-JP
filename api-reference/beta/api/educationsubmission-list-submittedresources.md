---
title: submittedresources を一覧表示する
description: 正式に提出されたリソースを一覧表示します。 提出物を所有する学生は、割り当てを再送信せずに、送信されたリストを変更することはできません。 これは、実際のリソースに関するラッパーであり、リソースが割り当てからコピーされた場合は、実際の割り当てリソースへのポインターを格納できます。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 021b167ae6991ce1ac799dcec4da21ac452fddb1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457672"
---
# <a name="list-submittedresources"></a><span data-ttu-id="b30ab-105">submittedresources を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b30ab-105">List submittedResources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b30ab-106">正式に提出されたリソースを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="b30ab-106">List the resources that have officially been submitted for grading.</span></span> <span data-ttu-id="b30ab-107">提出物を所有する学生は、割り当てを再送信せずに、送信されたリストを変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="b30ab-107">The student who owns the submission cannot change the submitted list without resubmitting the assignment.</span></span> <span data-ttu-id="b30ab-108">これは、実際のリソースに関するラッパーであり、リソースが割り当てからコピーされた場合は、実際の割り当てリソースへのポインターを格納できます。</span><span class="sxs-lookup"><span data-stu-id="b30ab-108">This is a wrapper around the real resource and can contain a pointer back to the actual assignment resource if this resource was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="b30ab-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b30ab-109">Permissions</span></span>
<span data-ttu-id="b30ab-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b30ab-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b30ab-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b30ab-112">Permission type</span></span>      | <span data-ttu-id="b30ab-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b30ab-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b30ab-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b30ab-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="b30ab-115">EduAssignments、EduAssignments、EduAssignments、および EduAssignments の読み取り/書き込みの基本</span><span class="sxs-lookup"><span data-stu-id="b30ab-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="b30ab-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b30ab-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b30ab-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b30ab-117">Not supported.</span></span>  |
|<span data-ttu-id="b30ab-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b30ab-118">Application</span></span> | <span data-ttu-id="b30ab-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b30ab-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b30ab-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b30ab-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b30ab-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b30ab-121">Optional query parameters</span></span>
<span data-ttu-id="b30ab-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b30ab-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b30ab-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b30ab-123">Request headers</span></span>
| <span data-ttu-id="b30ab-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b30ab-124">Header</span></span>       | <span data-ttu-id="b30ab-125">値</span><span class="sxs-lookup"><span data-stu-id="b30ab-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b30ab-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b30ab-126">Authorization</span></span>  | <span data-ttu-id="b30ab-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b30ab-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b30ab-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="b30ab-129">Request body</span></span>
<span data-ttu-id="b30ab-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b30ab-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b30ab-131">応答</span><span class="sxs-lookup"><span data-stu-id="b30ab-131">Response</span></span>
<span data-ttu-id="b30ab-132">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[educationSubmissionResource](../resources/educationsubmissionresource.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b30ab-132">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b30ab-133">例</span><span class="sxs-lookup"><span data-stu-id="b30ab-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b30ab-134">要求</span><span class="sxs-lookup"><span data-stu-id="b30ab-134">Request</span></span>
<span data-ttu-id="b30ab-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b30ab-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submittedresources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submittedResources
```
##### <a name="response"></a><span data-ttu-id="b30ab-136">応答</span><span class="sxs-lookup"><span data-stu-id="b30ab-136">Response</span></span>
<span data-ttu-id="b30ab-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b30ab-137">The following is an example of the response.</span></span> 

><span data-ttu-id="b30ab-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b30ab-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List submittedResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-list-submittedresources.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
