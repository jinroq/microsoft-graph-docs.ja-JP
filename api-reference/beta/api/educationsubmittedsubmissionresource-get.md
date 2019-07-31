---
title: EducationSubmittedSubmissionResource を取得する
description: 送信されたリソースを返します。 これは、学生が提出された後に教師が使用できるようになり、教師が提出をリリースした後に学生が使用できるようになります。  教師は一部のリソースにメモを残すことができますのでご注意ください。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f3703de6176af8cc475e83408d77d4880e2ef77b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954922"
---
# <a name="get-educationsubmittedsubmissionresource"></a><span data-ttu-id="307d3-105">EducationSubmittedSubmissionResource を取得する</span><span class="sxs-lookup"><span data-stu-id="307d3-105">Get educationSubmittedSubmissionResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="307d3-106">送信されたリソースを返します。</span><span class="sxs-lookup"><span data-stu-id="307d3-106">Returns a submitted resource.</span></span> <span data-ttu-id="307d3-107">これは、学生が提出された後に教師が使用できるようになり、教師が提出をリリースした後に学生が使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="307d3-107">This will be available to a teacher after a student has submitted, and will be available to the student after the teacher has released the submission.</span></span>  <span data-ttu-id="307d3-108">教師は一部のリソースにメモを残すことができますのでご注意ください。</span><span class="sxs-lookup"><span data-stu-id="307d3-108">Note that teachers can leave notes in some resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="307d3-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="307d3-109">Permissions</span></span>
<span data-ttu-id="307d3-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="307d3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="307d3-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="307d3-112">Permission type</span></span>      | <span data-ttu-id="307d3-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="307d3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="307d3-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="307d3-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="307d3-115">EduAssignments、EduAssignments、EduAssignments、および EduAssignments の読み取り/書き込みの基本</span><span class="sxs-lookup"><span data-stu-id="307d3-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="307d3-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="307d3-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="307d3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="307d3-117">Not supported.</span></span>  |
|<span data-ttu-id="307d3-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="307d3-118">Application</span></span> | <span data-ttu-id="307d3-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="307d3-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="307d3-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="307d3-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="307d3-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="307d3-121">Optional query parameters</span></span>
<span data-ttu-id="307d3-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="307d3-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="307d3-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="307d3-123">Request headers</span></span>
| <span data-ttu-id="307d3-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="307d3-124">Header</span></span>       | <span data-ttu-id="307d3-125">値</span><span class="sxs-lookup"><span data-stu-id="307d3-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="307d3-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="307d3-126">Authorization</span></span>  | <span data-ttu-id="307d3-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="307d3-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="307d3-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="307d3-129">Request body</span></span>
<span data-ttu-id="307d3-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="307d3-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="307d3-131">応答</span><span class="sxs-lookup"><span data-stu-id="307d3-131">Response</span></span>
<span data-ttu-id="307d3-132">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[educationSubmissionResource](../resources/educationsubmissionresource.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="307d3-132">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="307d3-133">例</span><span class="sxs-lookup"><span data-stu-id="307d3-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="307d3-134">要求</span><span class="sxs-lookup"><span data-stu-id="307d3-134">Request</span></span>
<span data-ttu-id="307d3-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="307d3-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmittedsubmissionresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submittedResources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="307d3-136">応答</span><span class="sxs-lookup"><span data-stu-id="307d3-136">Response</span></span>
<span data-ttu-id="307d3-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="307d3-137">The following is an example of the response.</span></span> 

><span data-ttu-id="307d3-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="307d3-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmittedSubmissionResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1152

{
  "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
  "id": "f2387c3b-ec39-4bf2-a399-d7242677f024",
  "resource": {
      "@odata.type": "#microsoft.graph.educationWordResource",
      "displayName": "Report.docx",
      "createdDateTime": "2017-10-21T07:52:53.9863696Z",
      "createdBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "lastModifiedDateTime": "2017-10-21T07:52:53.9863696Z",
      "lastModifiedBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeTZ_iul5AdW9f/items/017NJZI27BCN2QI2H7HJGLIVPXR6SD2DH6",
      "@odata.type": "microsoft.graph.educationResource"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationSubmittedSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
