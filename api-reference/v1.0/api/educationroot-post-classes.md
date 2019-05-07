---
title: Create educationClass
description: 新しいクラスを作成します。 これはユニバーサル グループも作成します。 この API を使用してクラスを作成すると、グループに特別なプロパティが追加されます。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: df8d289589e72800a65f7ac97cb9cd60020e1d1e
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33616312"
---
# <a name="create-educationclass"></a><span data-ttu-id="9d899-105">Create educationClass</span><span class="sxs-lookup"><span data-stu-id="9d899-105">Create educationClass</span></span>

<span data-ttu-id="9d899-106">新しいクラスを作成します。</span><span class="sxs-lookup"><span data-stu-id="9d899-106">Create a new class.</span></span> <span data-ttu-id="9d899-107">これはユニバーサル グループも作成します。</span><span class="sxs-lookup"><span data-stu-id="9d899-107">This will also create a universal group.</span></span> <span data-ttu-id="9d899-108">この API を使用してクラスを作成すると、Microsoft Teams 内に割り当てや特別な処理などの機能を追加する特別なプロパティがグループに追加されます。</span><span class="sxs-lookup"><span data-stu-id="9d899-108">When you use this API to create a class, it will add special properties to the group, which will add features such as assignments and special handling within Microsoft Teams.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d899-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9d899-109">Permissions</span></span>
<span data-ttu-id="9d899-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9d899-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d899-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9d899-112">Permission type</span></span>      | <span data-ttu-id="9d899-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9d899-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d899-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9d899-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="9d899-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d899-115">Not supported.</span></span>  |
|<span data-ttu-id="9d899-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9d899-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9d899-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d899-117">Not supported.</span></span>  |
|<span data-ttu-id="9d899-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9d899-118">Application</span></span> | <span data-ttu-id="9d899-119">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d899-119">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9d899-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9d899-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes
```
## <a name="request-headers"></a><span data-ttu-id="9d899-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9d899-121">Request headers</span></span>
| <span data-ttu-id="9d899-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9d899-122">Header</span></span>       | <span data-ttu-id="9d899-123">値</span><span class="sxs-lookup"><span data-stu-id="9d899-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9d899-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d899-124">Authorization</span></span>  | <span data-ttu-id="9d899-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9d899-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9d899-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9d899-127">Content-Type</span></span>  | <span data-ttu-id="9d899-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9d899-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9d899-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="9d899-129">Request body</span></span>
<span data-ttu-id="9d899-130">要求本文で、[educationClass](../resources/educationclass.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9d899-130">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="9d899-131">応答</span><span class="sxs-lookup"><span data-stu-id="9d899-131">Response</span></span>
<span data-ttu-id="9d899-132">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [educationClass](../resources/educationclass.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9d899-132">If successful, this method returns a `201 Created` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d899-133">例</span><span class="sxs-lookup"><span data-stu-id="9d899-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9d899-134">要求</span><span class="sxs-lookup"><span data-stu-id="9d899-134">Request</span></span>
<span data-ttu-id="9d899-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9d899-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes
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

##### <a name="response"></a><span data-ttu-id="9d899-136">応答</span><span class="sxs-lookup"><span data-stu-id="9d899-136">Response</span></span>
<span data-ttu-id="9d899-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9d899-137">The following is an example of the response.</span></span> 

><span data-ttu-id="9d899-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9d899-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="9d899-140">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="9d899-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9d899-141">Visual</span><span class="sxs-lookup"><span data-stu-id="9d899-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_educationclass_from_educationroot-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9d899-142">Java</span><span class="sxs-lookup"><span data-stu-id="9d899-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_educationclass_from_educationroot-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationroot-post-classes.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/educationroot-post-classes.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
