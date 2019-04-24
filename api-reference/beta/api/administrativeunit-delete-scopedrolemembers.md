---
title: scopedRoleMember を削除する
description: 管理単位からスコープ付き役割のメンバーを削除します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d373f9f88a6fba2f542abf8f58b751d05f3e75ae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459438"
---
# <a name="remove-a-scopedrolemember"></a><span data-ttu-id="5109a-103">scopedRoleMember を削除する</span><span class="sxs-lookup"><span data-stu-id="5109a-103">Remove a scopedRoleMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5109a-104">管理単位からスコープ付き役割のメンバーを削除します。</span><span class="sxs-lookup"><span data-stu-id="5109a-104">Remove a scoped-role member from an adminstrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="5109a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5109a-105">Permissions</span></span>
<span data-ttu-id="5109a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5109a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5109a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5109a-108">Permission type</span></span>      | <span data-ttu-id="5109a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5109a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5109a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5109a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5109a-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5109a-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5109a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5109a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5109a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5109a-113">Not supported.</span></span>    |
|<span data-ttu-id="5109a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5109a-114">Application</span></span> | <span data-ttu-id="5109a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5109a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5109a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5109a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/scopedRoleMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="5109a-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5109a-117">Request headers</span></span>
| <span data-ttu-id="5109a-118">名前</span><span class="sxs-lookup"><span data-stu-id="5109a-118">Name</span></span>       | <span data-ttu-id="5109a-119">説明</span><span class="sxs-lookup"><span data-stu-id="5109a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5109a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5109a-120">Authorization</span></span>  | <span data-ttu-id="5109a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5109a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5109a-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="5109a-123">Request body</span></span>
<span data-ttu-id="5109a-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5109a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5109a-125">応答</span><span class="sxs-lookup"><span data-stu-id="5109a-125">Response</span></span>

<span data-ttu-id="5109a-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="5109a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5109a-128">例</span><span class="sxs-lookup"><span data-stu-id="5109a-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5109a-129">要求</span><span class="sxs-lookup"><span data-stu-id="5109a-129">Request</span></span>
<span data-ttu-id="5109a-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5109a-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_scopedrolemember"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
##### <a name="response"></a><span data-ttu-id="5109a-131">応答</span><span class="sxs-lookup"><span data-stu-id="5109a-131">Response</span></span>
<span data-ttu-id="5109a-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5109a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-delete-scopedrolemembers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
