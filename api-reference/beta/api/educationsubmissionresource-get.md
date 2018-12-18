---
title: EducationSubmissionResource を取得します。
description: 提出書類に関連付けられている特定のリソースのプロパティを取得します。 このリソースでは、'作業' リソースの一覧では、学生によってプロセスでの作業を考慮する必要があります。 割り当てからコピーされた場合、このリソースは割り当てのリソースに使用可能なポインターがラップされます。
author: dipakboyed
ms.openlocfilehash: d7c1e6fcbe97a9a0a4c1735e37798097f2605b30
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361916"
---
# <a name="get-educationsubmissionresource"></a><span data-ttu-id="77581-105">EducationSubmissionResource を取得します。</span><span class="sxs-lookup"><span data-stu-id="77581-105">Get educationSubmissionResource</span></span>

> <span data-ttu-id="77581-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="77581-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77581-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77581-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="77581-108">提出書類に関連付けられている特定のリソースのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="77581-108">Retrieves the properties of a specific resource associated with the submission.</span></span> <span data-ttu-id="77581-109">このリソースは「処理中」リソース ボックスの一覧で、学生によってプロセスでの作業を考慮する必要があります。</span><span class="sxs-lookup"><span data-stu-id="77581-109">This resource is in the "working" resource list and should be considered work in process by a student.</span></span> <span data-ttu-id="77581-110">割り当てからコピーされた場合、このリソースは割り当てのリソースに使用可能なポインターがラップされます。</span><span class="sxs-lookup"><span data-stu-id="77581-110">This resource is wrapped with a possible pointer back to the assignment resource if it was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="77581-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="77581-111">Permissions</span></span>
<span data-ttu-id="77581-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="77581-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77581-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="77581-114">Permission type</span></span>      | <span data-ttu-id="77581-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="77581-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77581-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="77581-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="77581-117">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="77581-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="77581-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="77581-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="77581-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77581-119">Not supported.</span></span>  |
|<span data-ttu-id="77581-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="77581-120">Application</span></span> | <span data-ttu-id="77581-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77581-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="77581-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="77581-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="77581-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="77581-123">Optional query parameters</span></span>
<span data-ttu-id="77581-124">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="77581-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="77581-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="77581-125">Request headers</span></span>
| <span data-ttu-id="77581-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="77581-126">Header</span></span>       | <span data-ttu-id="77581-127">値</span><span class="sxs-lookup"><span data-stu-id="77581-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="77581-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="77581-128">Authorization</span></span>  | <span data-ttu-id="77581-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="77581-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="77581-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="77581-131">Request body</span></span>
<span data-ttu-id="77581-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="77581-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="77581-133">応答</span><span class="sxs-lookup"><span data-stu-id="77581-133">Response</span></span>
<span data-ttu-id="77581-134">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[educationSubmissionResource](../resources/educationsubmissionresource.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="77581-134">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="77581-135">例</span><span class="sxs-lookup"><span data-stu-id="77581-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="77581-136">要求</span><span class="sxs-lookup"><span data-stu-id="77581-136">Request</span></span>
<span data-ttu-id="77581-137">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="77581-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmissionresource"
}-->
```http 
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="77581-138">応答</span><span class="sxs-lookup"><span data-stu-id="77581-138">Response</span></span>
<span data-ttu-id="77581-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="77581-139">The following is an example of the response.</span></span> 

><span data-ttu-id="77581-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="77581-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmissionResource"
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
      "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeTZ_iul5AdW9f/items/017NJZI27BCN2QI2H7HJGLIVPXR6SD2DH6"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
