---
title: EducationAssignmentResource を作成します。
description: リソースの種類を示すために odata.type を作成しています。 ファイル ベースのリソースが割り当ての**resourceFolder**にアップロードする必要が最初に注意してください。
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 34e8740336acbef056ec0b3703547de51fdc42ce
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527991"
---
# <a name="create-educationassignmentresource"></a><span data-ttu-id="5bc6e-104">EducationAssignmentResource を作成します。</span><span class="sxs-lookup"><span data-stu-id="5bc6e-104">Create educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bc6e-105">[割り当てリソース](../resources/educationassignmentresource.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="5bc6e-105">Create an [assignment resource](../resources/educationassignmentresource.md).</span></span> <span data-ttu-id="5bc6e-106">リソース自体には、作成されるリソースの種類を示すために、@odata.type があります。</span><span class="sxs-lookup"><span data-stu-id="5bc6e-106">The resource itself has an @odata.type to indicate which type of resource is being created.</span></span> <span data-ttu-id="5bc6e-107">ファイル ベースのリソースが割り当ての**resourceFolder**にアップロードする必要が最初に注意してください。</span><span class="sxs-lookup"><span data-stu-id="5bc6e-107">Note that file-based resources must first be uploaded to the assignments **resourceFolder**.</span></span>

## <a name="permissions"></a><span data-ttu-id="5bc6e-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5bc6e-108">Permissions</span></span>
<span data-ttu-id="5bc6e-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5bc6e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bc6e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5bc6e-111">Permission type</span></span>      | <span data-ttu-id="5bc6e-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5bc6e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5bc6e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5bc6e-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="5bc6e-114">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5bc6e-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="5bc6e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5bc6e-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5bc6e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5bc6e-116">Not supported.</span></span>  |
|<span data-ttu-id="5bc6e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5bc6e-117">Application</span></span> | <span data-ttu-id="5bc6e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5bc6e-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="5bc6e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5bc6e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/resources
```
## <a name="request-headers"></a><span data-ttu-id="5bc6e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5bc6e-120">Request headers</span></span>
| <span data-ttu-id="5bc6e-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5bc6e-121">Header</span></span>       | <span data-ttu-id="5bc6e-122">値</span><span class="sxs-lookup"><span data-stu-id="5bc6e-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5bc6e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bc6e-123">Authorization</span></span>  | <span data-ttu-id="5bc6e-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5bc6e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5bc6e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5bc6e-126">Content-Type</span></span>  | <span data-ttu-id="5bc6e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5bc6e-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5bc6e-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="5bc6e-128">Request body</span></span>
<span data-ttu-id="5bc6e-129">要求の本文には、 [educationAssignmentResource](../resources/educationassignmentresource.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="5bc6e-129">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="5bc6e-130">応答</span><span class="sxs-lookup"><span data-stu-id="5bc6e-130">Response</span></span>
<span data-ttu-id="5bc6e-131">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文内の[educationAssignmentResource](../resources/educationassignmentresource.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="5bc6e-131">If successful, this method returns a `201 Created` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bc6e-132">例</span><span class="sxs-lookup"><span data-stu-id="5bc6e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5bc6e-133">要求</span><span class="sxs-lookup"><span data-stu-id="5bc6e-133">Request</span></span>
<span data-ttu-id="5bc6e-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5bc6e-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_educationassignmentresource_from_educationassignment"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources
Content-type: application/json
Content-length: 212

{
  "distributeForStudentWork": "false",
  "resource": {
    "displayName": "Bing",
    "link": "https://www.bing.com",
    "@odata.type": "#microsoft.education.assignments.api.educationLinkResource"
  }
}

```
<span data-ttu-id="5bc6e-135">要求の本文には、 [educationAssignmentResource](../resources/educationassignmentresource.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="5bc6e-135">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="5bc6e-136">応答</span><span class="sxs-lookup"><span data-stu-id="5bc6e-136">Response</span></span>
<span data-ttu-id="5bc6e-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5bc6e-137">The following is an example of the response.</span></span> 

><span data-ttu-id="5bc6e-138">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="5bc6e-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5bc6e-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5bc6e-139">All of the properties will be returned from an actual call.</span></span>


<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 229

{
  "id": "122333",
  "distributeForStudentWork": false,
  "resource": {
    "displayName": "Bing",
    "link": "https://www.bing.com",
    "@odata.type": "#microsoft.education.assignments.api.educationLinkResource"
  }
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-post-resources.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
