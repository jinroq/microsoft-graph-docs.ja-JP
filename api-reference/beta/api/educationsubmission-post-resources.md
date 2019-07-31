---
title: EducationSubmissionResource を作成する
description: 'リソースをリソースリストに追加します。 このアクションは、この送信を割り当てられている学生のみが実行できます。 **AllowStudentsToAddResources**フラグが true に設定されていない場合、このアクションは成功しません。 呼び出し元が新しいファイルベースのリソースを作成する場合は、提出物に関連付けられた resources フォルダーにファイルをアップロードする必要があります。 ファイルが存在しない場合、またはそのフォルダー内にない場合、POST 要求は失敗します。 '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 36b7f0432577dacb716c0eaa2ee232cc3e49a40e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955071"
---
# <a name="create-educationsubmissionresource"></a><span data-ttu-id="0aca8-107">EducationSubmissionResource を作成する</span><span class="sxs-lookup"><span data-stu-id="0aca8-107">Create educationSubmissionResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0aca8-108">リソースをリソースリストに追加します。</span><span class="sxs-lookup"><span data-stu-id="0aca8-108">Adds a resource to the resources list.</span></span> <span data-ttu-id="0aca8-109">このアクションは、この送信を割り当てられている学生のみが実行できます。</span><span class="sxs-lookup"><span data-stu-id="0aca8-109">This action can only be done by the student to whom this submission is assigned.</span></span> <span data-ttu-id="0aca8-110">**AllowStudentsToAddResources**フラグが true に設定されていない場合、このアクションは成功しません。</span><span class="sxs-lookup"><span data-stu-id="0aca8-110">This action will not succeed if the **allowStudentsToAddResources** flag is not set to true.</span></span> <span data-ttu-id="0aca8-111">呼び出し元が新しいファイルベースのリソースを作成する場合は、提出物に関連付けられた resources フォルダーにファイルをアップロードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="0aca8-111">If the caller wants to create a new file-based resource, the file must be uploaded to the resources folder that is associated with the submission.</span></span> <span data-ttu-id="0aca8-112">ファイルが存在しない場合、またはそのフォルダー内にない場合、POST 要求は失敗します。</span><span class="sxs-lookup"><span data-stu-id="0aca8-112">If the file does not exist or is not in that folder, the POST request will fail.</span></span> 

## <a name="permissions"></a><span data-ttu-id="0aca8-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0aca8-113">Permissions</span></span>
<span data-ttu-id="0aca8-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0aca8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0aca8-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0aca8-116">Permission type</span></span>      | <span data-ttu-id="0aca8-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0aca8-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0aca8-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0aca8-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="0aca8-119">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="0aca8-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="0aca8-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0aca8-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0aca8-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0aca8-121">Not supported.</span></span>  |
|<span data-ttu-id="0aca8-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0aca8-122">Application</span></span> | <span data-ttu-id="0aca8-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0aca8-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0aca8-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0aca8-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/resources

```
## <a name="request-headers"></a><span data-ttu-id="0aca8-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0aca8-125">Request headers</span></span>
| <span data-ttu-id="0aca8-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0aca8-126">Header</span></span>       | <span data-ttu-id="0aca8-127">値</span><span class="sxs-lookup"><span data-stu-id="0aca8-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0aca8-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="0aca8-128">Authorization</span></span>  | <span data-ttu-id="0aca8-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0aca8-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0aca8-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0aca8-131">Content-Type</span></span>  | <span data-ttu-id="0aca8-132">application/json</span><span class="sxs-lookup"><span data-stu-id="0aca8-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0aca8-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="0aca8-133">Request body</span></span>
<span data-ttu-id="0aca8-134">要求本文で、 [educationSubmissionResource](../resources/educationsubmissionresource.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0aca8-134">In the request body, supply a JSON representation of the [educationSubmissionResource](../resources/educationsubmissionresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="0aca8-135">応答</span><span class="sxs-lookup"><span data-stu-id="0aca8-135">Response</span></span>
<span data-ttu-id="0aca8-136">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[educationSubmissionResource](../resources/educationsubmissionresource.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0aca8-136">If successful, this method returns a `201 Created` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0aca8-137">例</span><span class="sxs-lookup"><span data-stu-id="0aca8-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0aca8-138">要求</span><span class="sxs-lookup"><span data-stu-id="0aca8-138">Request</span></span>
<span data-ttu-id="0aca8-139">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0aca8-139">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="0aca8-140">応答</span><span class="sxs-lookup"><span data-stu-id="0aca8-140">Response</span></span>
<span data-ttu-id="0aca8-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0aca8-141">The following is an example of the response.</span></span> 

><span data-ttu-id="0aca8-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0aca8-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "suppressions": []
}
-->
