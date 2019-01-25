---
title: Get administrativeUnit
description: この**educationSchool**に対応する単純なディレクトリ**administrativeUnit**を取得します。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 47dd3b5543f7f10385529aef56e99537abc2f524
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520705"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="122e9-103">Get administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="122e9-103">Get administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="122e9-104">この**educationSchool**に対応する単純なディレクトリ**administrativeUnit**を取得します。</span><span class="sxs-lookup"><span data-stu-id="122e9-104">Retrieve the simple directory **administrativeUnit** that corresponds to this **educationSchool**.</span></span>

><span data-ttu-id="122e9-105">**注:** 委任されたトークンを使用した場合、メンバーは自分の学校に関する情報以外を参照できません。</span><span class="sxs-lookup"><span data-stu-id="122e9-105">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="122e9-106">この場合は `...beta/education/me/schools` リソースを使用してください。</span><span class="sxs-lookup"><span data-stu-id="122e9-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="122e9-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="122e9-107">Permissions</span></span>
<span data-ttu-id="122e9-108">この API を呼び出すには、アクセス許可の組み合わせが必要です。</span><span class="sxs-lookup"><span data-stu-id="122e9-108">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="122e9-109">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="122e9-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="122e9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="122e9-110">Permission type</span></span>      | <span data-ttu-id="122e9-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="122e9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="122e9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="122e9-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="122e9-113">One from EduRoster.ReadBasic、EduRoster.Read、EduRoster.Write plus Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="122e9-113">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="122e9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="122e9-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="122e9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="122e9-115">Not supported.</span></span>  |
|<span data-ttu-id="122e9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="122e9-116">Application</span></span> | <span data-ttu-id="122e9-117">EduRoster.Read.All、EduRoster.ReadWrite.All plus Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="122e9-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="122e9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="122e9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/administrativeUnit
```
## <a name="request-headers"></a><span data-ttu-id="122e9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="122e9-119">Request headers</span></span>
| <span data-ttu-id="122e9-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="122e9-120">Header</span></span>       | <span data-ttu-id="122e9-121">値</span><span class="sxs-lookup"><span data-stu-id="122e9-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="122e9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="122e9-122">Authorization</span></span>  | <span data-ttu-id="122e9-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="122e9-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="122e9-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="122e9-125">Request body</span></span>
<span data-ttu-id="122e9-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="122e9-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="122e9-127">応答</span><span class="sxs-lookup"><span data-stu-id="122e9-127">Response</span></span>
<span data-ttu-id="122e9-128">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[administrativeUnit](../resources/administrativeunit.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="122e9-128">If successful, this method returns a `200 OK` response code and an [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="122e9-129">例</span><span class="sxs-lookup"><span data-stu-id="122e9-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="122e9-130">要求</span><span class="sxs-lookup"><span data-stu-id="122e9-130">Request</span></span>
<span data-ttu-id="122e9-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="122e9-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_administrativeUnit"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools/2961761D-8094-4183-A9F6-8E36E966C7D9/administrativeUnit
```
##### <a name="response"></a><span data-ttu-id="122e9-132">応答</span><span class="sxs-lookup"><span data-stu-id="122e9-132">Response</span></span>
<span data-ttu-id="122e9-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="122e9-133">The following is an example of the response.</span></span> 

><span data-ttu-id="122e9-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="122e9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value",
  "id": "id-value"
}
```

<!-- uuid: A681726F-B4A7-4BCF-9407-F87CB9A4771D
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationschool-get-administrativeUnit.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
