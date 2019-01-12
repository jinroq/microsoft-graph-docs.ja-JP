---
title: メンバー グループをチェックする
description: メンバーシップのグループ、およびそのリストから指定されたリスト内のそれらのグループを確認します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 93ff0a0cb215e489490e50bde40f56e5b562be95
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971089"
---
# <a name="check-member-groups"></a><span data-ttu-id="b2eed-103">メンバー グループをチェックする</span><span class="sxs-lookup"><span data-stu-id="b2eed-103">Check member groups</span></span>

> <span data-ttu-id="b2eed-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b2eed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2eed-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b2eed-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b2eed-106">グループ、およびそのリストからの指定されたリスト内のメンバーシップをそのグループのうち、指定したユーザー、グループ、サービス主体またはディレクトリ オブジェクトは、メンバーを確認します。</span><span class="sxs-lookup"><span data-stu-id="b2eed-106">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, service principal or directory object is a member.</span></span> <span data-ttu-id="b2eed-107">この関数は、推移的です。</span><span class="sxs-lookup"><span data-stu-id="b2eed-107">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2eed-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b2eed-108">Permissions</span></span>
<span data-ttu-id="b2eed-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b2eed-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b2eed-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b2eed-111">Permission type</span></span>      | <span data-ttu-id="b2eed-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b2eed-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2eed-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b2eed-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b2eed-114">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2eed-114">Directory.Read.All</span></span>    |
|<span data-ttu-id="b2eed-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b2eed-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2eed-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b2eed-116">Not supported.</span></span>    |
|<span data-ttu-id="b2eed-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b2eed-117">Application</span></span> | <span data-ttu-id="b2eed-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2eed-118">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2eed-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b2eed-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /servciePrincipals/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="b2eed-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b2eed-120">Request headers</span></span>
| <span data-ttu-id="b2eed-121">名前</span><span class="sxs-lookup"><span data-stu-id="b2eed-121">Name</span></span>       | <span data-ttu-id="b2eed-122">型</span><span class="sxs-lookup"><span data-stu-id="b2eed-122">Type</span></span> | <span data-ttu-id="b2eed-123">説明</span><span class="sxs-lookup"><span data-stu-id="b2eed-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b2eed-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2eed-124">Authorization</span></span>  | <span data-ttu-id="b2eed-125">string</span><span class="sxs-lookup"><span data-stu-id="b2eed-125">string</span></span>  | <span data-ttu-id="b2eed-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b2eed-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b2eed-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b2eed-128">Content-Type</span></span>  | <span data-ttu-id="b2eed-129">application/json</span><span class="sxs-lookup"><span data-stu-id="b2eed-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b2eed-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="b2eed-130">Request body</span></span>
<span data-ttu-id="b2eed-131">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="b2eed-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b2eed-132">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b2eed-132">Parameter</span></span>    | <span data-ttu-id="b2eed-133">型</span><span class="sxs-lookup"><span data-stu-id="b2eed-133">Type</span></span>   |<span data-ttu-id="b2eed-134">説明</span><span class="sxs-lookup"><span data-stu-id="b2eed-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2eed-135">groupIds</span><span class="sxs-lookup"><span data-stu-id="b2eed-135">groupIds</span></span>|<span data-ttu-id="b2eed-136">String</span><span class="sxs-lookup"><span data-stu-id="b2eed-136">String</span></span>|<span data-ttu-id="b2eed-p105">メンバーシップを確認するためのグループのオブジェクト ID を含むコレクションです。最大 20 グループを指定することが可能です。</span><span class="sxs-lookup"><span data-stu-id="b2eed-p105">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="b2eed-139">応答</span><span class="sxs-lookup"><span data-stu-id="b2eed-139">Response</span></span>

<span data-ttu-id="b2eed-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b2eed-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2eed-141">例</span><span class="sxs-lookup"><span data-stu-id="b2eed-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b2eed-142">要求</span><span class="sxs-lookup"><span data-stu-id="b2eed-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/checkMemberGroups
Content-type: application/json

{
  "groupIds": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="b2eed-143">応答</span><span class="sxs-lookup"><span data-stu-id="b2eed-143">Response</span></span>
<span data-ttu-id="b2eed-p106">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b2eed-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
