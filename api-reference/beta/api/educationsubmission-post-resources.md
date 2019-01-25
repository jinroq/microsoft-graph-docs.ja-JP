---
title: EducationSubmissionResource を作成します。
description: 'リソースを [リソース] リストに追加します。 このアクションは、この送信が割り当てられている受講者にのみ実行できます。 **AllowStudentsToAddResources**フラグが設定されていない場合、この操作は成功しません true に設定します。 呼び出し元は、ファイル ベースのリソースを新規作成する必要がある場合は、提出書類に関連付けられているリソース] フォルダーにファイルをアップロードする必要があります。 ファイルが存在しないか、そのフォルダーでは、POST 要求は失敗します。 '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: da0860d5b5f19a84643a05a88aaeb74651e2d8ea
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511731"
---
# <a name="create-educationsubmissionresource"></a><span data-ttu-id="dc12a-107">EducationSubmissionResource を作成します。</span><span class="sxs-lookup"><span data-stu-id="dc12a-107">Create educationSubmissionResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc12a-108">リソースを [リソース] リストに追加します。</span><span class="sxs-lookup"><span data-stu-id="dc12a-108">Adds a resource to the resources list.</span></span> <span data-ttu-id="dc12a-109">このアクションは、この送信が割り当てられている受講者にのみ実行できます。</span><span class="sxs-lookup"><span data-stu-id="dc12a-109">This action can only be done by the student to whom this submission is assigned.</span></span> <span data-ttu-id="dc12a-110">**AllowStudentsToAddResources**フラグが設定されていない場合、この操作は成功しません true に設定します。</span><span class="sxs-lookup"><span data-stu-id="dc12a-110">This action will not succeed if the **allowStudentsToAddResources** flag is not set to true.</span></span> <span data-ttu-id="dc12a-111">呼び出し元は、ファイル ベースのリソースを新規作成する必要がある場合は、提出書類に関連付けられているリソース] フォルダーにファイルをアップロードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="dc12a-111">If the caller wants to create a new file-based resource, the file must be uploaded to the resources folder that is associated with the submission.</span></span> <span data-ttu-id="dc12a-112">ファイルが存在しないか、そのフォルダーでは、POST 要求は失敗します。</span><span class="sxs-lookup"><span data-stu-id="dc12a-112">If the file does not exist or is not in that folder, the POST request will fail.</span></span> 

## <a name="permissions"></a><span data-ttu-id="dc12a-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dc12a-113">Permissions</span></span>
<span data-ttu-id="dc12a-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dc12a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc12a-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dc12a-116">Permission type</span></span>      | <span data-ttu-id="dc12a-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dc12a-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc12a-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dc12a-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="dc12a-119">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc12a-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="dc12a-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dc12a-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc12a-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc12a-121">Not supported.</span></span>  |
|<span data-ttu-id="dc12a-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dc12a-122">Application</span></span> | <span data-ttu-id="dc12a-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc12a-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="dc12a-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dc12a-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/resources

```
## <a name="request-headers"></a><span data-ttu-id="dc12a-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dc12a-125">Request headers</span></span>
| <span data-ttu-id="dc12a-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dc12a-126">Header</span></span>       | <span data-ttu-id="dc12a-127">値</span><span class="sxs-lookup"><span data-stu-id="dc12a-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dc12a-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc12a-128">Authorization</span></span>  | <span data-ttu-id="dc12a-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="dc12a-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dc12a-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dc12a-131">Content-Type</span></span>  | <span data-ttu-id="dc12a-132">application/json</span><span class="sxs-lookup"><span data-stu-id="dc12a-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dc12a-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="dc12a-133">Request body</span></span>
<span data-ttu-id="dc12a-134">要求の本文には、 [educationSubmissionResource](../resources/educationsubmissionresource.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="dc12a-134">In the request body, supply a JSON representation of the [educationSubmissionResource](../resources/educationsubmissionresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="dc12a-135">応答</span><span class="sxs-lookup"><span data-stu-id="dc12a-135">Response</span></span>
<span data-ttu-id="dc12a-136">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文内の[educationSubmissionResource](../resources/educationsubmissionresource.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="dc12a-136">If successful, this method returns a `201 Created` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc12a-137">例</span><span class="sxs-lookup"><span data-stu-id="dc12a-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dc12a-138">要求</span><span class="sxs-lookup"><span data-stu-id="dc12a-138">Request</span></span>
<span data-ttu-id="dc12a-139">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dc12a-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_educationsubmissionresource_from_educationsubmission"
}-->
```
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources
Content-type: application/json
Content-length: 1097

{
  "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
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
  },
  "@odata.type": "microsoft.graph.educationResource"
}

```

##### <a name="response"></a><span data-ttu-id="dc12a-140">応答</span><span class="sxs-lookup"><span data-stu-id="dc12a-140">Response</span></span>
<span data-ttu-id="dc12a-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dc12a-141">The following is an example of the response.</span></span> 

><span data-ttu-id="dc12a-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="dc12a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmissionResource"
} -->
```http
HTTP/1.1 201 Created
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
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-post-resources.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
