---
title: EducationAssignmentResource を作成する
description: odata。作成されるリソースの種類を示します。 ファイルベースのリソースは、まず、割り当てリソース**フォルダー**にアップロードする必要があることに注意してください。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 86cf738f7558814a76d07e7a7eb5ffd22d988d29
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955670"
---
# <a name="create-educationassignmentresource"></a><span data-ttu-id="91702-104">EducationAssignmentResource を作成する</span><span class="sxs-lookup"><span data-stu-id="91702-104">Create educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91702-105">[割り当てリソース](../resources/educationassignmentresource.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="91702-105">Create an [assignment resource](../resources/educationassignmentresource.md).</span></span> <span data-ttu-id="91702-106">リソース自体には、作成されるリソースの種類を示す @odata の種類があります。</span><span class="sxs-lookup"><span data-stu-id="91702-106">The resource itself has an @odata.type to indicate which type of resource is being created.</span></span> <span data-ttu-id="91702-107">ファイルベースのリソースは、まず、割り当てリソース**フォルダー**にアップロードする必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="91702-107">Note that file-based resources must first be uploaded to the assignments **resourceFolder**.</span></span>

## <a name="permissions"></a><span data-ttu-id="91702-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="91702-108">Permissions</span></span>
<span data-ttu-id="91702-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="91702-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91702-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="91702-111">Permission type</span></span>      | <span data-ttu-id="91702-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="91702-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91702-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="91702-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="91702-114">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="91702-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="91702-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="91702-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="91702-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91702-116">Not supported.</span></span>  |
|<span data-ttu-id="91702-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="91702-117">Application</span></span> | <span data-ttu-id="91702-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91702-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="91702-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="91702-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/resources
```
## <a name="request-headers"></a><span data-ttu-id="91702-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="91702-120">Request headers</span></span>
| <span data-ttu-id="91702-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="91702-121">Header</span></span>       | <span data-ttu-id="91702-122">値</span><span class="sxs-lookup"><span data-stu-id="91702-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="91702-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="91702-123">Authorization</span></span>  | <span data-ttu-id="91702-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="91702-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="91702-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="91702-126">Content-Type</span></span>  | <span data-ttu-id="91702-127">application/json</span><span class="sxs-lookup"><span data-stu-id="91702-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="91702-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="91702-128">Request body</span></span>
<span data-ttu-id="91702-129">要求本文で、 [educationAssignmentResource](../resources/educationassignmentresource.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="91702-129">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="91702-130">応答</span><span class="sxs-lookup"><span data-stu-id="91702-130">Response</span></span>
<span data-ttu-id="91702-131">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[educationAssignmentResource](../resources/educationassignmentresource.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="91702-131">If successful, this method returns a `201 Created` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91702-132">例</span><span class="sxs-lookup"><span data-stu-id="91702-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91702-133">要求</span><span class="sxs-lookup"><span data-stu-id="91702-133">Request</span></span>
<span data-ttu-id="91702-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="91702-134">The following is an example of the request.</span></span>
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
<span data-ttu-id="91702-135">要求本文で、 [educationAssignmentResource](../resources/educationassignmentresource.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="91702-135">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="91702-136">応答</span><span class="sxs-lookup"><span data-stu-id="91702-136">Response</span></span>
<span data-ttu-id="91702-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="91702-137">The following is an example of the response.</span></span> 

><span data-ttu-id="91702-138">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="91702-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="91702-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="91702-139">All of the properties will be returned from an actual call.</span></span>


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
  "suppressions": []
}
-->
