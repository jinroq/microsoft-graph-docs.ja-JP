---
title: educationSchool に educationUser を追加する
description: 学校にユーザーを追加します。
author: mmast-msft
ms.openlocfilehash: d7cabee054eddb6ac83bfdee5b0dea1ea25f9f36
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323080"
---
# <a name="add-educationuser-to-an-educationschool"></a><span data-ttu-id="256b7-103">educationSchool に educationUser を追加する</span><span class="sxs-lookup"><span data-stu-id="256b7-103">Add educationUser to an educationSchool</span></span>

<span data-ttu-id="256b7-104">学校にユーザーを追加します。</span><span class="sxs-lookup"><span data-stu-id="256b7-104">Add a user to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="256b7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="256b7-105">Permissions</span></span>
<span data-ttu-id="256b7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="256b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="256b7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="256b7-108">Permission type</span></span>      | <span data-ttu-id="256b7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="256b7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="256b7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="256b7-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="256b7-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="256b7-111">Not supported.</span></span>  |
|<span data-ttu-id="256b7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="256b7-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="256b7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="256b7-113">Not supported.</span></span>  |
|<span data-ttu-id="256b7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="256b7-114">Application</span></span> | <span data-ttu-id="256b7-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="256b7-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="256b7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="256b7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/users/$ref
```
## <a name="request-headers"></a><span data-ttu-id="256b7-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="256b7-117">Request headers</span></span>
| <span data-ttu-id="256b7-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="256b7-118">Header</span></span>       | <span data-ttu-id="256b7-119">値</span><span class="sxs-lookup"><span data-stu-id="256b7-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="256b7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="256b7-120">Authorization</span></span>  | <span data-ttu-id="256b7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="256b7-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="256b7-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="256b7-123">Content-Type</span></span>  | <span data-ttu-id="256b7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="256b7-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="256b7-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="256b7-125">Request body</span></span>
<span data-ttu-id="256b7-126">要求本文で、[educationUser](../resources/educationuser.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="256b7-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="256b7-127">応答</span><span class="sxs-lookup"><span data-stu-id="256b7-127">Response</span></span>
<span data-ttu-id="256b7-128">成功した場合、このメソッドは `204 No Content` 応答コードと、応答本文で [educationClass](../resources/educationclass.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="256b7-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="256b7-129">例</span><span class="sxs-lookup"><span data-stu-id="256b7-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="256b7-130">要求</span><span class="sxs-lookup"><span data-stu-id="256b7-130">Request</span></span>
<span data-ttu-id="256b7-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="256b7-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationschool"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/schools/{id}/users/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/v1.0/education/users/14008"
}
```

##### <a name="response"></a><span data-ttu-id="256b7-132">応答</span><span class="sxs-lookup"><span data-stu-id="256b7-132">Response</span></span>
<span data-ttu-id="256b7-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="256b7-133">The following is an example of the response.</span></span> 

<!-- Add the educationClass resource to the response. -->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->