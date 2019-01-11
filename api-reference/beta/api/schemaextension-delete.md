---
title: schemaExtension を削除する
description: スキーマ拡張機能の定義を削除します。
localization_priority: Normal
ms.openlocfilehash: 8641b00b984380592f14ae366b9cc20ab11dc7b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842197"
---
# <a name="delete-schemaextension"></a><span data-ttu-id="61390-103">schemaExtension を削除する</span><span class="sxs-lookup"><span data-stu-id="61390-103">Delete schemaExtension</span></span>

> <span data-ttu-id="61390-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="61390-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61390-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61390-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="61390-106">[スキーマ拡張機能](../resources/schemaextension.md)の定義を削除します。</span><span class="sxs-lookup"><span data-stu-id="61390-106">Delete the definition of a [schema extension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="61390-p102">スキーマ拡張機能を作成したアプリ (所有者アプリ) だけが、そのスキーマ拡張機能が **InDevelopment** 状態の場合に限り、スキーマ拡張機能の定義を削除できます。スキーマ拡張機能の定義を削除しても、その定義に基づいてリソース インスタンスに追加されたカスタム データへのアクセスには影響しません。</span><span class="sxs-lookup"><span data-stu-id="61390-p102">Only the app that created the schema extension (owner app) can delete the schema extension definition, and only when the extension is in the **InDevelopment** state. Deleting a schema extension definition does not affect accessing custom data that has been added to resource instances based on that definition.</span></span>


## <a name="permissions"></a><span data-ttu-id="61390-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="61390-109">Permissions</span></span>
<span data-ttu-id="61390-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="61390-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="61390-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="61390-112">Permission type</span></span>      | <span data-ttu-id="61390-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="61390-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61390-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="61390-114">Delegated (work or school account)</span></span> | <span data-ttu-id="61390-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="61390-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="61390-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="61390-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61390-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61390-117">Not supported.</span></span>    |
|<span data-ttu-id="61390-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="61390-118">Application</span></span> | <span data-ttu-id="61390-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61390-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="61390-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="61390-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="61390-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="61390-121">Request headers</span></span>
| <span data-ttu-id="61390-122">名前</span><span class="sxs-lookup"><span data-stu-id="61390-122">Name</span></span>      |<span data-ttu-id="61390-123">説明</span><span class="sxs-lookup"><span data-stu-id="61390-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="61390-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="61390-124">Authorization</span></span>  | <span data-ttu-id="61390-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="61390-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61390-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="61390-127">Request body</span></span>
<span data-ttu-id="61390-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="61390-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61390-129">応答</span><span class="sxs-lookup"><span data-stu-id="61390-129">Response</span></span>

<span data-ttu-id="61390-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="61390-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61390-132">例</span><span class="sxs-lookup"><span data-stu-id="61390-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="61390-133">要求</span><span class="sxs-lookup"><span data-stu-id="61390-133">Request</span></span>
<span data-ttu-id="61390-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="61390-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/schemaExtensions/{id}
```
##### <a name="response"></a><span data-ttu-id="61390-135">応答</span><span class="sxs-lookup"><span data-stu-id="61390-135">Response</span></span>
<span data-ttu-id="61390-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="61390-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="61390-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="61390-137">See also</span></span>

- [<span data-ttu-id="61390-138">拡張機能を使用したリソースへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="61390-138">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="61390-139">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="61390-139">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
