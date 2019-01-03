---
title: EducationAssignmentResource を作成します。
description: リソースの種類を示すために odata.type を作成しています。 ファイル ベースのリソースが割り当ての**resourceFolder**にアップロードする必要が最初に注意してください。
ms.openlocfilehash: a2bb810d16c2d0a46fc2e2f4a5938b5779df24af
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068326"
---
# <a name="create-educationassignmentresource"></a><span data-ttu-id="8e6b8-104">EducationAssignmentResource を作成します。</span><span class="sxs-lookup"><span data-stu-id="8e6b8-104">Create educationAssignmentResource</span></span>

> <span data-ttu-id="8e6b8-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8e6b8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e6b8-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e6b8-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8e6b8-107">[割り当てリソース](../resources/educationassignmentresource.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="8e6b8-107">Create an [assignment resource](../resources/educationassignmentresource.md).</span></span> <span data-ttu-id="8e6b8-108">リソース自体には、作成されるリソースの種類を示すために、@odata.type があります。</span><span class="sxs-lookup"><span data-stu-id="8e6b8-108">The resource itself has an @odata.type to indicate which type of resource is being created.</span></span> <span data-ttu-id="8e6b8-109">ファイル ベースのリソースが割り当ての**resourceFolder**にアップロードする必要が最初に注意してください。</span><span class="sxs-lookup"><span data-stu-id="8e6b8-109">Note that file-based resources must first be uploaded to the assignments **resourceFolder**.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e6b8-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8e6b8-110">Permissions</span></span>
<span data-ttu-id="8e6b8-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8e6b8-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e6b8-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8e6b8-113">Permission type</span></span>      | <span data-ttu-id="8e6b8-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8e6b8-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e6b8-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8e6b8-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="8e6b8-116">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e6b8-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="8e6b8-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8e6b8-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8e6b8-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e6b8-118">Not supported.</span></span>  |
|<span data-ttu-id="8e6b8-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8e6b8-119">Application</span></span> | <span data-ttu-id="8e6b8-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e6b8-120">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="8e6b8-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8e6b8-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/resources
```
## <a name="request-headers"></a><span data-ttu-id="8e6b8-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8e6b8-122">Request headers</span></span>
| <span data-ttu-id="8e6b8-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8e6b8-123">Header</span></span>       | <span data-ttu-id="8e6b8-124">値</span><span class="sxs-lookup"><span data-stu-id="8e6b8-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8e6b8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e6b8-125">Authorization</span></span>  | <span data-ttu-id="8e6b8-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8e6b8-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8e6b8-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8e6b8-128">Content-Type</span></span>  | <span data-ttu-id="8e6b8-129">application/json</span><span class="sxs-lookup"><span data-stu-id="8e6b8-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8e6b8-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="8e6b8-130">Request body</span></span>
<span data-ttu-id="8e6b8-131">要求の本文には、 [educationAssignmentResource](../resources/educationassignmentresource.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="8e6b8-131">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="8e6b8-132">応答</span><span class="sxs-lookup"><span data-stu-id="8e6b8-132">Response</span></span>
<span data-ttu-id="8e6b8-133">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文内の[educationAssignmentResource](../resources/educationassignmentresource.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="8e6b8-133">If successful, this method returns a `201 Created` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e6b8-134">例</span><span class="sxs-lookup"><span data-stu-id="8e6b8-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8e6b8-135">要求</span><span class="sxs-lookup"><span data-stu-id="8e6b8-135">Request</span></span>
<span data-ttu-id="8e6b8-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8e6b8-136">The following is an example of the request.</span></span>
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
<span data-ttu-id="8e6b8-137">要求の本文には、 [educationAssignmentResource](../resources/educationassignmentresource.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="8e6b8-137">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8e6b8-138">応答</span><span class="sxs-lookup"><span data-stu-id="8e6b8-138">Response</span></span>
<span data-ttu-id="8e6b8-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8e6b8-139">The following is an example of the response.</span></span> 

><span data-ttu-id="8e6b8-140">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="8e6b8-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8e6b8-141">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8e6b8-141">All of the properties will be returned from an actual call.</span></span>


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
<!-- {
  "type": "#page.annotation",
  "description": "Create educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->