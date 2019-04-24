---
title: メンバー グループをチェックする
description: 指定したグループの一覧のメンバーシップを確認し、それらのグループをリストから返します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 53c89a6dd6fb0c16e0df7c6035ed0667c227787d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455192"
---
# <a name="check-member-groups"></a><span data-ttu-id="c3ace-103">メンバー グループをチェックする</span><span class="sxs-lookup"><span data-stu-id="c3ace-103">Check member groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3ace-104">指定したグループの一覧のメンバーシップを確認し、指定されたユーザー、グループ、サービスプリンシパル、またはディレクトリオブジェクトがメンバーであるグループをリストから返します。</span><span class="sxs-lookup"><span data-stu-id="c3ace-104">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, service principal or directory object is a member.</span></span> <span data-ttu-id="c3ace-105">この関数は、推移的です。</span><span class="sxs-lookup"><span data-stu-id="c3ace-105">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3ace-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c3ace-106">Permissions</span></span>
<span data-ttu-id="c3ace-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3ace-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c3ace-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c3ace-109">Permission type</span></span>      | <span data-ttu-id="c3ace-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c3ace-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3ace-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c3ace-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c3ace-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3ace-112">Directory.Read.All</span></span>    |
|<span data-ttu-id="c3ace-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c3ace-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3ace-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3ace-114">Not supported.</span></span>    |
|<span data-ttu-id="c3ace-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c3ace-115">Application</span></span> | <span data-ttu-id="c3ace-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3ace-116">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3ace-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c3ace-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /servciePrincipals/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="c3ace-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3ace-118">Request headers</span></span>
| <span data-ttu-id="c3ace-119">名前</span><span class="sxs-lookup"><span data-stu-id="c3ace-119">Name</span></span>       | <span data-ttu-id="c3ace-120">型</span><span class="sxs-lookup"><span data-stu-id="c3ace-120">Type</span></span> | <span data-ttu-id="c3ace-121">説明</span><span class="sxs-lookup"><span data-stu-id="c3ace-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c3ace-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3ace-122">Authorization</span></span>  | <span data-ttu-id="c3ace-123">string</span><span class="sxs-lookup"><span data-stu-id="c3ace-123">string</span></span>  | <span data-ttu-id="c3ace-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c3ace-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c3ace-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c3ace-126">Content-Type</span></span>  | <span data-ttu-id="c3ace-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c3ace-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c3ace-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="c3ace-128">Request body</span></span>
<span data-ttu-id="c3ace-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="c3ace-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c3ace-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c3ace-130">Parameter</span></span>    | <span data-ttu-id="c3ace-131">型</span><span class="sxs-lookup"><span data-stu-id="c3ace-131">Type</span></span>   |<span data-ttu-id="c3ace-132">説明</span><span class="sxs-lookup"><span data-stu-id="c3ace-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3ace-133">groupIds</span><span class="sxs-lookup"><span data-stu-id="c3ace-133">groupIds</span></span>|<span data-ttu-id="c3ace-134">String</span><span class="sxs-lookup"><span data-stu-id="c3ace-134">String</span></span>|<span data-ttu-id="c3ace-p104">メンバーシップを確認するためのグループのオブジェクト ID を含むコレクションです。最大 20 グループを指定することが可能です。</span><span class="sxs-lookup"><span data-stu-id="c3ace-p104">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="c3ace-137">応答</span><span class="sxs-lookup"><span data-stu-id="c3ace-137">Response</span></span>

<span data-ttu-id="c3ace-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c3ace-138">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3ace-139">例</span><span class="sxs-lookup"><span data-stu-id="c3ace-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c3ace-140">要求</span><span class="sxs-lookup"><span data-stu-id="c3ace-140">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="c3ace-141">応答</span><span class="sxs-lookup"><span data-stu-id="c3ace-141">Response</span></span>
<span data-ttu-id="c3ace-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c3ace-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryobject-checkmembergroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
