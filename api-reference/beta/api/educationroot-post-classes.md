---
title: Create educationClass
description: 新しいクラスを作成します。 これはユニバーサル グループも作成します。 クラスを作成するのにはこの API を使用すると特別なプロパティがどのグループに追加されます。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 6a5097777392184508c6d7be6f19a198c1c5bbd9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965132"
---
# <a name="create-educationclass"></a><span data-ttu-id="5776a-105">Create educationClass</span><span class="sxs-lookup"><span data-stu-id="5776a-105">Create educationClass</span></span>

> <span data-ttu-id="5776a-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5776a-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5776a-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5776a-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5776a-108">新しいクラスを作成します。</span><span class="sxs-lookup"><span data-stu-id="5776a-108">Create a new class.</span></span> <span data-ttu-id="5776a-109">これはユニバーサル グループも作成します。</span><span class="sxs-lookup"><span data-stu-id="5776a-109">This will also create a universal group.</span></span> <span data-ttu-id="5776a-110">この API を使用してクラスを作成すると、Microsoft Teams 内に割り当てや特別な処理などの機能を追加する特別なプロパティがグループに追加されます。</span><span class="sxs-lookup"><span data-stu-id="5776a-110">When you use this API to create a class, it will add special properties to the group, which will add features such as assignments and special handling within Microsoft Teams.</span></span>

## <a name="permissions"></a><span data-ttu-id="5776a-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5776a-111">Permissions</span></span>
<span data-ttu-id="5776a-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5776a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5776a-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5776a-114">Permission type</span></span>      | <span data-ttu-id="5776a-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5776a-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5776a-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5776a-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="5776a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5776a-117">Not supported.</span></span>  |
|<span data-ttu-id="5776a-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5776a-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5776a-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5776a-119">Not supported.</span></span>  |
|<span data-ttu-id="5776a-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5776a-120">Application</span></span> | <span data-ttu-id="5776a-121">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5776a-121">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5776a-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5776a-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes
```
## <a name="request-headers"></a><span data-ttu-id="5776a-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5776a-123">Request headers</span></span>
| <span data-ttu-id="5776a-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5776a-124">Header</span></span>       | <span data-ttu-id="5776a-125">値</span><span class="sxs-lookup"><span data-stu-id="5776a-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5776a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="5776a-126">Authorization</span></span>  | <span data-ttu-id="5776a-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5776a-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5776a-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5776a-129">Content-Type</span></span>  | <span data-ttu-id="5776a-130">application/json</span><span class="sxs-lookup"><span data-stu-id="5776a-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5776a-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="5776a-131">Request body</span></span>
<span data-ttu-id="5776a-132">要求本文で、[educationClass](../resources/educationclass.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5776a-132">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="5776a-133">応答</span><span class="sxs-lookup"><span data-stu-id="5776a-133">Response</span></span>
<span data-ttu-id="5776a-134">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [educationClass](../resources/educationclass.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5776a-134">If successful, this method returns a `201 Created` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5776a-135">例</span><span class="sxs-lookup"><span data-stu-id="5776a-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5776a-136">要求</span><span class="sxs-lookup"><span data-stu-id="5776a-136">Request</span></span>
<span data-ttu-id="5776a-137">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5776a-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes
Content-type: application/json
Content-length: 224

{
  "description": "Health Level 1",
  "classCode": "Health 501",
  "displayName": "Health 1",
  "externalId": "11019",
  "externalName": "Health Level 1",
  "externalSource": "sis",
  "mailNickname": "fineartschool.net"
}
```

##### <a name="response"></a><span data-ttu-id="5776a-138">応答</span><span class="sxs-lookup"><span data-stu-id="5776a-138">Response</span></span>
<span data-ttu-id="5776a-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5776a-139">The following is an example of the response.</span></span> 

><span data-ttu-id="5776a-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5776a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 224

{
    "id": "11019",
    "description": "Health Level 1",
    "classCode": "Health 501",
    "createdBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012",
      }
    },
    "displayName": "Health 1",
    "externalId": "11019",
    "externalName": "Health Level 1",
    "externalSource": "sis",
    "mailNickname": "fineartschool.net"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
