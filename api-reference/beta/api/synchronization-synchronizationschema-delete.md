---
title: 同期スキーマの削除
description: カスタマイズされたスキーマを削除し、スキーマを既定の構成にリセットします。 スキーマがテンプレートのコンテキストで削除されると、そのテンプレートに関連付けられている既定のスキーマにリセット`factoryTag`されます。
localization_priority: Normal
ms.openlocfilehash: cb4c6295fe962ea9570da19b9b6ee8190b2024f5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545346"
---
# <a name="delete-synchronizationschema"></a><span data-ttu-id="4d94b-104">同期スキーマの削除</span><span class="sxs-lookup"><span data-stu-id="4d94b-104">Delete synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d94b-105">カスタマイズされたスキーマを削除し、スキーマを既定の構成にリセットします。</span><span class="sxs-lookup"><span data-stu-id="4d94b-105">Deletes the customized schema and resets the schema to the default configuration.</span></span> <span data-ttu-id="4d94b-106">スキーマがテンプレートのコンテキストで削除されると、そのテンプレートに関連付けられている既定のスキーマにリセット`factoryTag`されます。</span><span class="sxs-lookup"><span data-stu-id="4d94b-106">If the schema is deleted in the context of the template, it resets the schema to the default one associated with the template's `factoryTag`.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d94b-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4d94b-107">Permissions</span></span>
<span data-ttu-id="4d94b-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d94b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d94b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4d94b-110">Permission type</span></span>                        | <span data-ttu-id="4d94b-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4d94b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d94b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4d94b-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="4d94b-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d94b-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="4d94b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4d94b-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="4d94b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d94b-115">Not supported.</span></span>|
|<span data-ttu-id="4d94b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4d94b-116">Application</span></span>                            |<span data-ttu-id="4d94b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d94b-117">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="4d94b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4d94b-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
DELETE /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="4d94b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4d94b-119">Request headers</span></span>

| <span data-ttu-id="4d94b-120">名前</span><span class="sxs-lookup"><span data-stu-id="4d94b-120">Name</span></span>           | <span data-ttu-id="4d94b-121">型</span><span class="sxs-lookup"><span data-stu-id="4d94b-121">Type</span></span>    | <span data-ttu-id="4d94b-122">説明</span><span class="sxs-lookup"><span data-stu-id="4d94b-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="4d94b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d94b-123">Authorization</span></span>  | <span data-ttu-id="4d94b-124">string</span><span class="sxs-lookup"><span data-stu-id="4d94b-124">string</span></span>  | <span data-ttu-id="4d94b-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4d94b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d94b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4d94b-127">Request body</span></span>

<span data-ttu-id="4d94b-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4d94b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d94b-129">応答</span><span class="sxs-lookup"><span data-stu-id="4d94b-129">Response</span></span>

<span data-ttu-id="4d94b-130">成功した場合、このメソッドは `201 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="4d94b-130">If successful, this method returns a `201 No Content` response code.</span></span> <span data-ttu-id="4d94b-131">応答本文では何も返しません。</span><span class="sxs-lookup"><span data-stu-id="4d94b-131">It does not return anything in response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d94b-132">例</span><span class="sxs-lookup"><span data-stu-id="4d94b-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4d94b-133">要求</span><span class="sxs-lookup"><span data-stu-id="4d94b-133">Request</span></span>
<span data-ttu-id="4d94b-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4d94b-134">The following is an example of a request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="4d94b-135">応答</span><span class="sxs-lookup"><span data-stu-id="4d94b-135">Response</span></span>
<span data-ttu-id="4d94b-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4d94b-136">The following is an example of a response.</span></span>
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
  "description": "Delete synchronizationSchema",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
