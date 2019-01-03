---
title: Get administrativeUnit
description: この**educationSchool**に対応する単純なディレクトリ**administrativeUnit**を取得します。
ms.openlocfilehash: 49ac05b44bc89f827091c3b846885a58cb7b8956
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070666"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="f600b-103">Get administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="f600b-103">Get administrativeUnit</span></span>

> <span data-ttu-id="f600b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f600b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f600b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f600b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f600b-106">この**educationSchool**に対応する単純なディレクトリ**administrativeUnit**を取得します。</span><span class="sxs-lookup"><span data-stu-id="f600b-106">Retrieve the simple directory **administrativeUnit** that corresponds to this **educationSchool**.</span></span>

><span data-ttu-id="f600b-107">**注:** 委任されたトークンを使用した場合、メンバーは自分の学校に関する情報以外を参照できません。</span><span class="sxs-lookup"><span data-stu-id="f600b-107">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="f600b-108">この場合は `...beta/education/me/schools` リソースを使用してください。</span><span class="sxs-lookup"><span data-stu-id="f600b-108">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="f600b-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f600b-109">Permissions</span></span>
<span data-ttu-id="f600b-110">この API を呼び出すには、アクセス許可の組み合わせが必要です。</span><span class="sxs-lookup"><span data-stu-id="f600b-110">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="f600b-111">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f600b-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f600b-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f600b-112">Permission type</span></span>      | <span data-ttu-id="f600b-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f600b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f600b-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f600b-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="f600b-115">One from EduRoster.ReadBasic、EduRoster.Read、EduRoster.Write plus Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f600b-115">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="f600b-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f600b-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f600b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f600b-117">Not supported.</span></span>  |
|<span data-ttu-id="f600b-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f600b-118">Application</span></span> | <span data-ttu-id="f600b-119">EduRoster.Read.All、EduRoster.ReadWrite.All plus Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f600b-119">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="f600b-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f600b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/administrativeUnit
```
## <a name="request-headers"></a><span data-ttu-id="f600b-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f600b-121">Request headers</span></span>
| <span data-ttu-id="f600b-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f600b-122">Header</span></span>       | <span data-ttu-id="f600b-123">値</span><span class="sxs-lookup"><span data-stu-id="f600b-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f600b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f600b-124">Authorization</span></span>  | <span data-ttu-id="f600b-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f600b-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f600b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f600b-127">Request body</span></span>
<span data-ttu-id="f600b-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f600b-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f600b-129">応答</span><span class="sxs-lookup"><span data-stu-id="f600b-129">Response</span></span>
<span data-ttu-id="f600b-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[administrativeUnit](../resources/administrativeunit.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f600b-130">If successful, this method returns a `200 OK` response code and an [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f600b-131">例</span><span class="sxs-lookup"><span data-stu-id="f600b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f600b-132">要求</span><span class="sxs-lookup"><span data-stu-id="f600b-132">Request</span></span>
<span data-ttu-id="f600b-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f600b-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_administrativeUnit"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools/2961761D-8094-4183-A9F6-8E36E966C7D9/administrativeUnit
```
##### <a name="response"></a><span data-ttu-id="f600b-134">応答</span><span class="sxs-lookup"><span data-stu-id="f600b-134">Response</span></span>
<span data-ttu-id="f600b-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f600b-135">The following is an example of the response.</span></span> 

><span data-ttu-id="f600b-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f600b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->