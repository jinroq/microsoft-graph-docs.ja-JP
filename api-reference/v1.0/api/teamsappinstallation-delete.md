---
title: チームからアプリケーションを削除します。
description: 指定されたチームからアプリケーションをアンインストールします。
ms.openlocfilehash: a1ba2ce7234796e3a2df508d40432a15690b1a63
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021183"
---
# <a name="delete-app-from-team"></a><span data-ttu-id="7ec55-103">チームからアプリケーションを削除します。</span><span class="sxs-lookup"><span data-stu-id="7ec55-103">Delete app from team</span></span>



<span data-ttu-id="7ec55-104">指定された[チーム](../resources/team.md)から[アプリケーション](../resources/teamsappinstallation.md)をアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="7ec55-104">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7ec55-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7ec55-105">Permissions</span></span>
<span data-ttu-id="7ec55-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7ec55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ec55-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7ec55-108">Permission type</span></span>      | <span data-ttu-id="7ec55-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7ec55-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ec55-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7ec55-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7ec55-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ec55-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7ec55-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7ec55-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ec55-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ec55-113">Not supported.</span></span>    |
|<span data-ttu-id="7ec55-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7ec55-114">Application</span></span> | <span data-ttu-id="7ec55-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ec55-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ec55-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7ec55-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7ec55-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7ec55-117">Request headers</span></span>
| <span data-ttu-id="7ec55-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7ec55-118">Header</span></span>       | <span data-ttu-id="7ec55-119">値</span><span class="sxs-lookup"><span data-stu-id="7ec55-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7ec55-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ec55-120">Authorization</span></span>  | <span data-ttu-id="7ec55-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7ec55-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7ec55-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="7ec55-123">Request body</span></span>
<span data-ttu-id="7ec55-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7ec55-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ec55-125">応答</span><span class="sxs-lookup"><span data-stu-id="7ec55-125">Response</span></span>

<span data-ttu-id="7ec55-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="7ec55-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ec55-128">例</span><span class="sxs-lookup"><span data-stu-id="7ec55-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7ec55-129">要求</span><span class="sxs-lookup"><span data-stu-id="7ec55-129">Request</span></span>
<span data-ttu-id="7ec55-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7ec55-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}
```
#### <a name="response"></a><span data-ttu-id="7ec55-131">応答</span><span class="sxs-lookup"><span data-stu-id="7ec55-131">Response</span></span>
<span data-ttu-id="7ec55-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7ec55-132">The following is an example of the response.</span></span> <span data-ttu-id="7ec55-133">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="7ec55-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7ec55-134">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7ec55-134">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
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
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->