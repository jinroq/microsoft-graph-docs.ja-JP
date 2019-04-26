---
title: チームを更新する
description: 指定されたチームのプロパティを更新します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a6dd8e38261cb2e64c3717ea3bee26ca96bd8958
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548993"
---
# <a name="update-team"></a><span data-ttu-id="16bc9-103">チームを更新する</span><span class="sxs-lookup"><span data-stu-id="16bc9-103">Update team</span></span>



<span data-ttu-id="16bc9-104">指定した[チーム](../resources/team.md)のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="16bc9-104">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="16bc9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="16bc9-105">Permissions</span></span>
<span data-ttu-id="16bc9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="16bc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="16bc9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="16bc9-108">Permission type</span></span>      | <span data-ttu-id="16bc9-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="16bc9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16bc9-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="16bc9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="16bc9-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16bc9-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="16bc9-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="16bc9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16bc9-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16bc9-113">Not supported.</span></span>    |
|<span data-ttu-id="16bc9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="16bc9-114">Application</span></span> | <span data-ttu-id="16bc9-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16bc9-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="16bc9-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="16bc9-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="16bc9-117">グローバル管理者と Microsoft Teams サービス管理者は、メンバーではないチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="16bc9-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="16bc9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="16bc9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```

## <a name="request-headers"></a><span data-ttu-id="16bc9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16bc9-119">Request headers</span></span>
| <span data-ttu-id="16bc9-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16bc9-120">Header</span></span>       | <span data-ttu-id="16bc9-121">値</span><span class="sxs-lookup"><span data-stu-id="16bc9-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="16bc9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="16bc9-122">Authorization</span></span>  | <span data-ttu-id="16bc9-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="16bc9-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="16bc9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="16bc9-125">Content-Type</span></span>  | <span data-ttu-id="16bc9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="16bc9-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="16bc9-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="16bc9-127">Request body</span></span>
<span data-ttu-id="16bc9-128">要求本文で、 [team](../resources/team.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="16bc9-128">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="16bc9-129">応答</span><span class="sxs-lookup"><span data-stu-id="16bc9-129">Response</span></span>

<span data-ttu-id="16bc9-130">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="16bc9-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="16bc9-131">例</span><span class="sxs-lookup"><span data-stu-id="16bc9-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="16bc9-132">要求</span><span class="sxs-lookup"><span data-stu-id="16bc9-132">Request</span></span>
<span data-ttu-id="16bc9-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="16bc9-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_team"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/teams/{id}
Content-type: application/json
Content-length: 211

{  
  "memberSettings": {
    "allowCreateUpdateChannels": true
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict"
  }
}
```
#### <a name="response"></a><span data-ttu-id="16bc9-134">応答</span><span class="sxs-lookup"><span data-stu-id="16bc9-134">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
