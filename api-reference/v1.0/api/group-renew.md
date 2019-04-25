---
title: 'group: renew'
description: グループの有効期限を更新します。 グループが更新されると、グループの有効期限はポリシーで定義された日数、延長されます。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 46a51d0a1d4bea5cebc4c3178f6776d80f313fbd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579010"
---
# <a name="group-renew"></a><span data-ttu-id="41820-104">group: renew</span><span class="sxs-lookup"><span data-stu-id="41820-104">group: renew</span></span>

<span data-ttu-id="41820-105">グループの有効期限を更新します。</span><span class="sxs-lookup"><span data-stu-id="41820-105">Renews a group's expiration.</span></span> <span data-ttu-id="41820-106">グループが更新されると、グループの有効期限はポリシーで定義された日数、延長されます。</span><span class="sxs-lookup"><span data-stu-id="41820-106">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="41820-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="41820-107">Permissions</span></span>

<span data-ttu-id="41820-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41820-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="41820-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="41820-110">Permission type</span></span>      | <span data-ttu-id="41820-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="41820-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41820-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="41820-112">Delegated (work or school account)</span></span> | <span data-ttu-id="41820-113">Group.ReadWrite.All または Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41820-113">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="41820-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="41820-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41820-115">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="41820-115">Not supported</span></span> |
|<span data-ttu-id="41820-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="41820-116">Application</span></span> | <span data-ttu-id="41820-117">Group.ReadWrite.All または Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41820-117">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="41820-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="41820-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/renew
```

## <a name="request-headers"></a><span data-ttu-id="41820-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="41820-119">Request headers</span></span>
| <span data-ttu-id="41820-120">名前</span><span class="sxs-lookup"><span data-stu-id="41820-120">Name</span></span>       | <span data-ttu-id="41820-121">説明</span><span class="sxs-lookup"><span data-stu-id="41820-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="41820-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="41820-122">Authorization</span></span>  | <span data-ttu-id="41820-123">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="41820-123">Bearer {token}</span></span> |


## <a name="request-body"></a><span data-ttu-id="41820-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="41820-124">Request body</span></span>

<span data-ttu-id="41820-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="41820-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41820-126">応答</span><span class="sxs-lookup"><span data-stu-id="41820-126">Response</span></span>

<span data-ttu-id="41820-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="41820-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41820-129">例</span><span class="sxs-lookup"><span data-stu-id="41820-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="41820-130">要求</span><span class="sxs-lookup"><span data-stu-id="41820-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "group_renew"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/renew
```

##### <a name="response"></a><span data-ttu-id="41820-131">応答</span><span class="sxs-lookup"><span data-stu-id="41820-131">Response</span></span>
<span data-ttu-id="41820-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="41820-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Boolean"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: renew",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
