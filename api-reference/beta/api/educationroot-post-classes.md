---
title: Create educationClass
description: 新しいクラスを作成します。 これはユニバーサル グループも作成します。 クラスを作成するのにはこの API を使用すると特別なプロパティがどのグループに追加されます。
ms.openlocfilehash: 81b72b5b252c323a6a91152deaafaf8a927c8bf9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066361"
---
# <a name="create-educationclass"></a><span data-ttu-id="9f48b-105">Create educationClass</span><span class="sxs-lookup"><span data-stu-id="9f48b-105">Create educationClass</span></span>

> <span data-ttu-id="9f48b-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9f48b-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f48b-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f48b-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9f48b-108">新しいクラスを作成します。</span><span class="sxs-lookup"><span data-stu-id="9f48b-108">Create a new class.</span></span> <span data-ttu-id="9f48b-109">これはユニバーサル グループも作成します。</span><span class="sxs-lookup"><span data-stu-id="9f48b-109">This will also create a universal group.</span></span> <span data-ttu-id="9f48b-110">この API を使用してクラスを作成すると、Microsoft Teams 内に割り当てや特別な処理などの機能を追加する特別なプロパティがグループに追加されます。</span><span class="sxs-lookup"><span data-stu-id="9f48b-110">When you use this API to create a class, it will add special properties to the group, which will add features such as assignments and special handling within Microsoft Teams.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f48b-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9f48b-111">Permissions</span></span>
<span data-ttu-id="9f48b-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9f48b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f48b-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9f48b-114">Permission type</span></span>      | <span data-ttu-id="9f48b-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9f48b-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f48b-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9f48b-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="9f48b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f48b-117">Not supported.</span></span>  |
|<span data-ttu-id="9f48b-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9f48b-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9f48b-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f48b-119">Not supported.</span></span>  |
|<span data-ttu-id="9f48b-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9f48b-120">Application</span></span> | <span data-ttu-id="9f48b-121">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f48b-121">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9f48b-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9f48b-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes
```
## <a name="request-headers"></a><span data-ttu-id="9f48b-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9f48b-123">Request headers</span></span>
| <span data-ttu-id="9f48b-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9f48b-124">Header</span></span>       | <span data-ttu-id="9f48b-125">値</span><span class="sxs-lookup"><span data-stu-id="9f48b-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9f48b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f48b-126">Authorization</span></span>  | <span data-ttu-id="9f48b-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9f48b-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9f48b-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9f48b-129">Content-Type</span></span>  | <span data-ttu-id="9f48b-130">application/json</span><span class="sxs-lookup"><span data-stu-id="9f48b-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9f48b-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="9f48b-131">Request body</span></span>
<span data-ttu-id="9f48b-132">要求本文で、[educationClass](../resources/educationclass.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9f48b-132">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="9f48b-133">応答</span><span class="sxs-lookup"><span data-stu-id="9f48b-133">Response</span></span>
<span data-ttu-id="9f48b-134">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [educationClass](../resources/educationclass.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9f48b-134">If successful, this method returns a `201 Created` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f48b-135">例</span><span class="sxs-lookup"><span data-stu-id="9f48b-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f48b-136">要求</span><span class="sxs-lookup"><span data-stu-id="9f48b-136">Request</span></span>
<span data-ttu-id="9f48b-137">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9f48b-137">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="9f48b-138">応答</span><span class="sxs-lookup"><span data-stu-id="9f48b-138">Response</span></span>
<span data-ttu-id="9f48b-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9f48b-139">The following is an example of the response.</span></span> 

><span data-ttu-id="9f48b-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9f48b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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