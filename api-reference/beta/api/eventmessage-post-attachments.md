---
title: 添付ファイルを追加する
description: この API を使用して、新しい添付ファイルを作成します。
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: e56da5a4b6f57506800e07e3f8e2b09ed7ef6f46
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824081"
---
# <a name="add-attachment"></a><span data-ttu-id="81e6c-103">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="81e6c-103">Add attachment</span></span>

> <span data-ttu-id="81e6c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="81e6c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81e6c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81e6c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="81e6c-106">この API を使用して、新しい添付ファイルを作成します。</span><span class="sxs-lookup"><span data-stu-id="81e6c-106">Use this API to create a new Attachment.</span></span>

<span data-ttu-id="81e6c-107">添付ファイルは、次の種類のいずれかにできます。</span><span class="sxs-lookup"><span data-stu-id="81e6c-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="81e6c-108">ファイル ([fileAttachment](../resources/fileattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="81e6c-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="81e6c-109">項目 ([itemAttachment](../resources/itemattachment.md) リソースで表される連絡先、イベント、メッセージ)。</span><span class="sxs-lookup"><span data-stu-id="81e6c-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="81e6c-110">ファイルへのリンク ([referenceAttachment](../resources/referenceattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="81e6c-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="81e6c-111">これらの添付ファイル リソースのすべての種類は、[attachment](../resources/attachment.md) リソースから派生します。</span><span class="sxs-lookup"><span data-stu-id="81e6c-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="81e6c-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="81e6c-112">Permissions</span></span>
<span data-ttu-id="81e6c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="81e6c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81e6c-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="81e6c-115">Permission type</span></span>      | <span data-ttu-id="81e6c-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="81e6c-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81e6c-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="81e6c-117">Delegated (work or school account)</span></span> | <span data-ttu-id="81e6c-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81e6c-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="81e6c-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="81e6c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81e6c-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81e6c-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="81e6c-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="81e6c-121">Application</span></span> | <span data-ttu-id="81e6c-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81e6c-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="81e6c-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="81e6c-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id|userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="81e6c-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="81e6c-124">Request headers</span></span>
| <span data-ttu-id="81e6c-125">名前</span><span class="sxs-lookup"><span data-stu-id="81e6c-125">Name</span></span>       | <span data-ttu-id="81e6c-126">種類</span><span class="sxs-lookup"><span data-stu-id="81e6c-126">Type</span></span> | <span data-ttu-id="81e6c-127">説明</span><span class="sxs-lookup"><span data-stu-id="81e6c-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="81e6c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="81e6c-128">Authorization</span></span>  | <span data-ttu-id="81e6c-129">string</span><span class="sxs-lookup"><span data-stu-id="81e6c-129">string</span></span>  | <span data-ttu-id="81e6c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="81e6c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="81e6c-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="81e6c-132">Content-Type</span></span> | <span data-ttu-id="81e6c-133">string</span><span class="sxs-lookup"><span data-stu-id="81e6c-133">string</span></span>  | <span data-ttu-id="81e6c-p104">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="81e6c-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="81e6c-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="81e6c-136">Request body</span></span>
<span data-ttu-id="81e6c-137">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="81e6c-137">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="81e6c-138">応答</span><span class="sxs-lookup"><span data-stu-id="81e6c-138">Response</span></span>

<span data-ttu-id="81e6c-139">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="81e6c-139">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="81e6c-140">例 (添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="81e6c-140">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="81e6c-141">要求</span><span class="sxs-lookup"><span data-stu-id="81e6c-141">Request</span></span>
<span data-ttu-id="81e6c-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="81e6c-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/{id}/attachments
Content-type: application/json

{
  "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
  "name": "name-value",
  "contentType": "contentType-value",
  "isInline": false,
  "contentLocation": "contentLocation-value",
  "contentBytes": "contentBytes-value"
}
```

##### <a name="response"></a><span data-ttu-id="81e6c-143">応答</span><span class="sxs-lookup"><span data-stu-id="81e6c-143">Response</span></span>
<span data-ttu-id="81e6c-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="81e6c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
```


## <a name="example-item-attachment"></a><span data-ttu-id="81e6c-147">例 (項目の添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="81e6c-147">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="81e6c-148">要求</span><span class="sxs-lookup"><span data-stu-id="81e6c-148">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/attachments
Content-type: application/json

{
  "@odata.type": "#Microsoft.OutlookServices.ItemAttachment",
  "name": "name-value",
  "item": "message or event entity"
}
```

##### <a name="response"></a><span data-ttu-id="81e6c-149">応答</span><span class="sxs-lookup"><span data-stu-id="81e6c-149">Response</span></span>
<span data-ttu-id="81e6c-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="81e6c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
