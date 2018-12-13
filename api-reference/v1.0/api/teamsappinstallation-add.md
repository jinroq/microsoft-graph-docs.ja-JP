---
title: アプリケーションをチームに追加します。
description: 指定されたチームには、アプリケーションをインストールします。
ms.openlocfilehash: ec03c0f8744bd2f1dd5cf5e2a7e84c9b59a7c6ce
ms.sourcegitcommit: ba6b1d1a12dcb54916b4d3e529c856f6514e01e7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/12/2018
ms.locfileid: "27241035"
---
# <a name="add-app-to-team"></a><span data-ttu-id="144bd-103">アプリケーションをチームに追加します。</span><span class="sxs-lookup"><span data-stu-id="144bd-103">Add app to team</span></span>



<span data-ttu-id="144bd-104">指定された[チーム](../resources/team.md)には、[アプリケーション](../resources/teamsapp.md)をインストールします。</span><span class="sxs-lookup"><span data-stu-id="144bd-104">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="144bd-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="144bd-105">Permissions</span></span>
<span data-ttu-id="144bd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="144bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="144bd-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="144bd-108">Permission type</span></span>      | <span data-ttu-id="144bd-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="144bd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="144bd-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="144bd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="144bd-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="144bd-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="144bd-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="144bd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="144bd-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="144bd-113">Not supported.</span></span>    |
|<span data-ttu-id="144bd-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="144bd-114">Application</span></span> | <span data-ttu-id="144bd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="144bd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="144bd-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="144bd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="144bd-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="144bd-117">Request headers</span></span>
| <span data-ttu-id="144bd-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="144bd-118">Header</span></span>       | <span data-ttu-id="144bd-119">値</span><span class="sxs-lookup"><span data-stu-id="144bd-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="144bd-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="144bd-120">Authorization</span></span>  | <span data-ttu-id="144bd-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="144bd-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="144bd-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="144bd-123">Request body</span></span>

| <span data-ttu-id="144bd-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="144bd-124">Property</span></span>     | <span data-ttu-id="144bd-125">種類</span><span class="sxs-lookup"><span data-stu-id="144bd-125">Type</span></span>   |<span data-ttu-id="144bd-126">説明</span><span class="sxs-lookup"><span data-stu-id="144bd-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="144bd-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="144bd-127">teamsApp</span></span>| [<span data-ttu-id="144bd-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="144bd-128">teamsApp</span></span>](../resources/teamsapp.md) |<span data-ttu-id="144bd-129">追加するアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="144bd-129">The app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="144bd-130">応答</span><span class="sxs-lookup"><span data-stu-id="144bd-130">Response</span></span>

<span data-ttu-id="144bd-131">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="144bd-131">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="144bd-132">例</span><span class="sxs-lookup"><span data-stu-id="144bd-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="144bd-133">要求</span><span class="sxs-lookup"><span data-stu-id="144bd-133">Request</span></span>
<span data-ttu-id="144bd-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="144bd-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST /teams/{id}/installedApps
{
   "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
#### <a name="response"></a><span data-ttu-id="144bd-135">応答</span><span class="sxs-lookup"><span data-stu-id="144bd-135">Response</span></span>
<span data-ttu-id="144bd-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="144bd-136">The following is an example of the response.</span></span> <span data-ttu-id="144bd-137">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="144bd-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="144bd-138">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="144bd-138">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
}
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

## <a name="see-also"></a><span data-ttu-id="144bd-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="144bd-139">See also</span></span>

