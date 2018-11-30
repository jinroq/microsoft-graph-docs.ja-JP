---
title: EducationSubmissionResource を作成します。
description: 'リソースを [リソース] リストに追加します。 このアクションは、この送信が割り当てられている受講者にのみ実行できます。 **AllowStudentsToAddResources**フラグが設定されていない場合、この操作は成功しません true に設定します。 呼び出し元は、ファイル ベースのリソースを新規作成する必要がある場合は、提出書類に関連付けられているリソース] フォルダーにファイルをアップロードする必要があります。 ファイルが存在しないか、そのフォルダーでは、POST 要求は失敗します。 '
ms.openlocfilehash: c49022cc8ff830ad4842901be8a678875ea9b2a3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073134"
---
# <a name="create-educationsubmissionresource"></a><span data-ttu-id="5e5a2-107">EducationSubmissionResource を作成します。</span><span class="sxs-lookup"><span data-stu-id="5e5a2-107">Create educationSubmissionResource</span></span>

> <span data-ttu-id="5e5a2-108">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5e5a2-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e5a2-109">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5e5a2-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5e5a2-110">リソースを [リソース] リストに追加します。</span><span class="sxs-lookup"><span data-stu-id="5e5a2-110">Adds a resource to the resources list.</span></span> <span data-ttu-id="5e5a2-111">このアクションは、この送信が割り当てられている受講者にのみ実行できます。</span><span class="sxs-lookup"><span data-stu-id="5e5a2-111">This action can only be done by the student to whom this submission is assigned.</span></span> <span data-ttu-id="5e5a2-112">**AllowStudentsToAddResources**フラグが設定されていない場合、この操作は成功しません true に設定します。</span><span class="sxs-lookup"><span data-stu-id="5e5a2-112">This action will not succeed if the **allowStudentsToAddResources** flag is not set to true.</span></span> <span data-ttu-id="5e5a2-113">呼び出し元は、ファイル ベースのリソースを新規作成する必要がある場合は、提出書類に関連付けられているリソース] フォルダーにファイルをアップロードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="5e5a2-113">If the caller wants to create a new file-based resource, the file must be uploaded to the resources folder that is associated with the submission.</span></span> <span data-ttu-id="5e5a2-114">ファイルが存在しないか、そのフォルダーでは、POST 要求は失敗します。</span><span class="sxs-lookup"><span data-stu-id="5e5a2-114">If the file does not exist or is not in that folder, the POST request will fail.</span></span> 

## <a name="permissions"></a><span data-ttu-id="5e5a2-115">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5e5a2-115">Permissions</span></span>
<span data-ttu-id="5e5a2-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5e5a2-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e5a2-118">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5e5a2-118">Permission type</span></span>      | <span data-ttu-id="5e5a2-119">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5e5a2-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e5a2-120">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5e5a2-120">Delegated (work or school account)</span></span> |  <span data-ttu-id="5e5a2-121">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e5a2-121">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="5e5a2-122">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5e5a2-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e5a2-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5e5a2-123">Not supported.</span></span>  |
|<span data-ttu-id="5e5a2-124">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5e5a2-124">Application</span></span> | <span data-ttu-id="5e5a2-125">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5e5a2-125">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5e5a2-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5e5a2-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/resources

```
## <a name="request-headers"></a><span data-ttu-id="5e5a2-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5e5a2-127">Request headers</span></span>
| <span data-ttu-id="5e5a2-128">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5e5a2-128">Header</span></span>       | <span data-ttu-id="5e5a2-129">値</span><span class="sxs-lookup"><span data-stu-id="5e5a2-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5e5a2-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e5a2-130">Authorization</span></span>  | <span data-ttu-id="5e5a2-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5e5a2-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5e5a2-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5e5a2-133">Content-Type</span></span>  | <span data-ttu-id="5e5a2-134">application/json</span><span class="sxs-lookup"><span data-stu-id="5e5a2-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5e5a2-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="5e5a2-135">Request body</span></span>
<span data-ttu-id="5e5a2-136">要求の本文には、 [educationSubmissionResource](../resources/educationsubmissionresource.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="5e5a2-136">In the request body, supply a JSON representation of the [educationSubmissionResource](../resources/educationsubmissionresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="5e5a2-137">応答</span><span class="sxs-lookup"><span data-stu-id="5e5a2-137">Response</span></span>
<span data-ttu-id="5e5a2-138">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文内の[educationSubmissionResource](../resources/educationsubmissionresource.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="5e5a2-138">If successful, this method returns a `201 Created` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e5a2-139">例</span><span class="sxs-lookup"><span data-stu-id="5e5a2-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5e5a2-140">要求</span><span class="sxs-lookup"><span data-stu-id="5e5a2-140">Request</span></span>
<span data-ttu-id="5e5a2-141">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5e5a2-141">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="5e5a2-142">応答</span><span class="sxs-lookup"><span data-stu-id="5e5a2-142">Response</span></span>
<span data-ttu-id="5e5a2-143">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5e5a2-143">The following is an example of the response.</span></span> 

><span data-ttu-id="5e5a2-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5e5a2-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Create educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->