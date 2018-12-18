---
title: 生徒を追加する
description: クラスにメンバーを追加します。
author: mmast-msft
ms.openlocfilehash: 112bfd3ff67dfe2dde42f8e51c015640662a4006
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313686"
---
# <a name="add-a-student"></a><span data-ttu-id="d9278-103">生徒を追加する</span><span class="sxs-lookup"><span data-stu-id="d9278-103">Add a student</span></span>

<span data-ttu-id="d9278-104">クラスにメンバーを追加します。</span><span class="sxs-lookup"><span data-stu-id="d9278-104">Add a member to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9278-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d9278-105">Permissions</span></span>
<span data-ttu-id="d9278-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d9278-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9278-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d9278-108">Permission type</span></span>      | <span data-ttu-id="d9278-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d9278-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9278-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d9278-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="d9278-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9278-111">Not supported.</span></span>  |
|<span data-ttu-id="d9278-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d9278-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d9278-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9278-113">Not supported.</span></span>  |
|<span data-ttu-id="d9278-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d9278-114">Application</span></span> | <span data-ttu-id="d9278-115">EduRoster.ReadWrite.All と Member.Read.Hidden</span><span class="sxs-lookup"><span data-stu-id="d9278-115">EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d9278-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d9278-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="d9278-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d9278-117">Request headers</span></span>
| <span data-ttu-id="d9278-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d9278-118">Header</span></span>       | <span data-ttu-id="d9278-119">値</span><span class="sxs-lookup"><span data-stu-id="d9278-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d9278-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9278-120">Authorization</span></span>  | <span data-ttu-id="d9278-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d9278-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d9278-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d9278-123">Content-Type</span></span>  | <span data-ttu-id="d9278-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d9278-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d9278-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d9278-125">Request body</span></span>
<span data-ttu-id="d9278-126">要求本文で、[educationUser](../resources/educationuser.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d9278-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="d9278-127">応答</span><span class="sxs-lookup"><span data-stu-id="d9278-127">Response</span></span>
<span data-ttu-id="d9278-128">成功した場合、このメソッドは `204 No Content` 応答コードと、応答本文で [educationClass](../resources/educationclass.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d9278-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9278-129">例</span><span class="sxs-lookup"><span data-stu-id="d9278-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d9278-130">要求</span><span class="sxs-lookup"><span data-stu-id="d9278-130">Request</span></span>
<span data-ttu-id="d9278-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d9278-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/{class-id}/members/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/v1.0/education/users/13015"
}
```

##### <a name="response"></a><span data-ttu-id="d9278-132">応答</span><span class="sxs-lookup"><span data-stu-id="d9278-132">Response</span></span>
<span data-ttu-id="d9278-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d9278-133">The following is an example of the response.</span></span> 


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
