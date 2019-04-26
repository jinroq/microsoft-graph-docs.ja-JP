---
title: educationAssignmentResource を作成する
description: odata。作成されるリソースの種類を示します。 ファイルベースのリソースは、まず、割り当てリソース**フォルダー**にアップロードする必要があることに注意してください。
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 408ff1b44fda0d4e9b6f16c2234ed06a4ca24852
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324709"
---
# <a name="create-educationassignmentresource"></a><span data-ttu-id="80e52-104">educationAssignmentResource を作成する</span><span class="sxs-lookup"><span data-stu-id="80e52-104">Create educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80e52-105">[割り当てリソース](../resources/educationassignmentresource.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="80e52-105">Create an [assignment resource](../resources/educationassignmentresource.md).</span></span> <span data-ttu-id="80e52-106">リソース自体には、作成されるリソースの種類を示す @odata の種類があります。</span><span class="sxs-lookup"><span data-stu-id="80e52-106">The resource itself has an @odata.type to indicate which type of resource is being created.</span></span> <span data-ttu-id="80e52-107">ファイルベースのリソースは、まず、割り当てリソース**フォルダー**にアップロードする必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="80e52-107">Note that file-based resources must first be uploaded to the assignments **resourceFolder**.</span></span>

## <a name="permissions"></a><span data-ttu-id="80e52-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="80e52-108">Permissions</span></span>
<span data-ttu-id="80e52-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="80e52-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80e52-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="80e52-111">Permission type</span></span>      | <span data-ttu-id="80e52-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="80e52-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80e52-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="80e52-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="80e52-114">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="80e52-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="80e52-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="80e52-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="80e52-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80e52-116">Not supported.</span></span>  |
|<span data-ttu-id="80e52-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="80e52-117">Application</span></span> | <span data-ttu-id="80e52-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80e52-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="80e52-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="80e52-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/resources
```
## <a name="request-headers"></a><span data-ttu-id="80e52-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="80e52-120">Request headers</span></span>
| <span data-ttu-id="80e52-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="80e52-121">Header</span></span>       | <span data-ttu-id="80e52-122">値</span><span class="sxs-lookup"><span data-stu-id="80e52-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="80e52-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="80e52-123">Authorization</span></span>  | <span data-ttu-id="80e52-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="80e52-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="80e52-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="80e52-126">Content-Type</span></span>  | <span data-ttu-id="80e52-127">application/json</span><span class="sxs-lookup"><span data-stu-id="80e52-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="80e52-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="80e52-128">Request body</span></span>
<span data-ttu-id="80e52-129">要求本文で、 [educationAssignmentResource](../resources/educationassignmentresource.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="80e52-129">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="80e52-130">応答</span><span class="sxs-lookup"><span data-stu-id="80e52-130">Response</span></span>
<span data-ttu-id="80e52-131">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[educationAssignmentResource](../resources/educationassignmentresource.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="80e52-131">If successful, this method returns a `201 Created` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80e52-132">例</span><span class="sxs-lookup"><span data-stu-id="80e52-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="80e52-133">要求</span><span class="sxs-lookup"><span data-stu-id="80e52-133">Request</span></span>
<span data-ttu-id="80e52-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="80e52-134">The following is an example of the request.</span></span>
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
<span data-ttu-id="80e52-135">要求本文で、 [educationAssignmentResource](../resources/educationassignmentresource.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="80e52-135">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="80e52-136">応答</span><span class="sxs-lookup"><span data-stu-id="80e52-136">Response</span></span>
<span data-ttu-id="80e52-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="80e52-137">The following is an example of the response.</span></span> 

><span data-ttu-id="80e52-138">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="80e52-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="80e52-139">すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="80e52-139">All of the properties will be returned from an actual call.</span></span>


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
