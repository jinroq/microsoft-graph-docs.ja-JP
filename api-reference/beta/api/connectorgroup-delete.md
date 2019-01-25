---
title: ConnectorGroup を削除します。
description: ConnectorGroup を削除します。
localization_priority: Normal
ms.openlocfilehash: a0fd138281b8337df49388f4a10dc34cc02da18d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516029"
---
# <a name="delete-connectorgroup"></a><span data-ttu-id="0507f-103">ConnectorGroup を削除します。</span><span class="sxs-lookup"><span data-stu-id="0507f-103">Delete connectorGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0507f-104">ConnectorGroup を削除します。</span><span class="sxs-lookup"><span data-stu-id="0507f-104">Delete a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="0507f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0507f-105">Permissions</span></span>
<span data-ttu-id="0507f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0507f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0507f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0507f-108">Permission type</span></span>      | <span data-ttu-id="0507f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0507f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0507f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0507f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0507f-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0507f-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0507f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0507f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0507f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0507f-113">Not supported.</span></span>    |
|<span data-ttu-id="0507f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0507f-114">Application</span></span> | <span data-ttu-id="0507f-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0507f-115">Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="0507f-116">**注:** コネクタ グループには、それに関連するすべてのコネクタが必要ありません。</span><span class="sxs-lookup"><span data-stu-id="0507f-116">**Note:** The connector group must not have any connectors associated with it.</span></span>

## <a name="http-request"></a><span data-ttu-id="0507f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0507f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /connectorGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0507f-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0507f-118">Request headers</span></span>
| <span data-ttu-id="0507f-119">名前</span><span class="sxs-lookup"><span data-stu-id="0507f-119">Name</span></span>       | <span data-ttu-id="0507f-120">説明</span><span class="sxs-lookup"><span data-stu-id="0507f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0507f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0507f-121">Authorization</span></span>  | <span data-ttu-id="0507f-122">Bearer </span><span class="sxs-lookup"><span data-stu-id="0507f-122">Bearer.</span></span> <span data-ttu-id="0507f-123">必須</span><span class="sxs-lookup"><span data-stu-id="0507f-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="0507f-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="0507f-124">Request body</span></span>
<span data-ttu-id="0507f-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0507f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0507f-126">応答</span><span class="sxs-lookup"><span data-stu-id="0507f-126">Response</span></span>

<span data-ttu-id="0507f-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="0507f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0507f-129">例</span><span class="sxs-lookup"><span data-stu-id="0507f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0507f-130">要求</span><span class="sxs-lookup"><span data-stu-id="0507f-130">Request</span></span>
<span data-ttu-id="0507f-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0507f-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_connectorgroup"
}-->
```http
DELETE https://graph.microsoft.com/{ver}/connectorGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="0507f-132">応答</span><span class="sxs-lookup"><span data-stu-id="0507f-132">Response</span></span>
<span data-ttu-id="0507f-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0507f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/connectorgroup-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
