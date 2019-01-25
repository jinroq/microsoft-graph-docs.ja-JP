---
title: 添付ファイルを追加する
description: この API を使用して、新しい添付ファイルを作成します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 504b3daccc5e1313ee56d23a87b2d25eb62abae9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522666"
---
# <a name="add-attachment"></a><span data-ttu-id="81789-103">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="81789-103">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81789-104">この API を使用して、新しい添付ファイルを作成します。</span><span class="sxs-lookup"><span data-stu-id="81789-104">Use this API to create a new Attachment.</span></span>

<span data-ttu-id="81789-105">添付ファイルは、次の種類のいずれかにできます。</span><span class="sxs-lookup"><span data-stu-id="81789-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="81789-106">ファイル ([fileAttachment](../resources/fileattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="81789-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="81789-107">項目 ([itemAttachment](../resources/itemattachment.md) リソースで表される連絡先、イベント、メッセージ)。</span><span class="sxs-lookup"><span data-stu-id="81789-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="81789-108">ファイルへのリンク ([referenceAttachment](../resources/referenceattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="81789-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="81789-109">これらの添付ファイル リソースのすべての種類は、[attachment](../resources/attachment.md) リソースから派生します。</span><span class="sxs-lookup"><span data-stu-id="81789-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="81789-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="81789-110">Permissions</span></span>
<span data-ttu-id="81789-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="81789-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81789-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="81789-113">Permission type</span></span>      | <span data-ttu-id="81789-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="81789-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81789-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="81789-115">Delegated (work or school account)</span></span> | <span data-ttu-id="81789-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81789-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="81789-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="81789-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81789-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81789-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="81789-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="81789-119">Application</span></span> | <span data-ttu-id="81789-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81789-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="81789-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="81789-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id|userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="81789-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="81789-122">Request headers</span></span>
| <span data-ttu-id="81789-123">名前</span><span class="sxs-lookup"><span data-stu-id="81789-123">Name</span></span>       | <span data-ttu-id="81789-124">型</span><span class="sxs-lookup"><span data-stu-id="81789-124">Type</span></span> | <span data-ttu-id="81789-125">説明</span><span class="sxs-lookup"><span data-stu-id="81789-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="81789-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="81789-126">Authorization</span></span>  | <span data-ttu-id="81789-127">string</span><span class="sxs-lookup"><span data-stu-id="81789-127">string</span></span>  | <span data-ttu-id="81789-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="81789-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="81789-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="81789-130">Content-Type</span></span> | <span data-ttu-id="81789-131">string</span><span class="sxs-lookup"><span data-stu-id="81789-131">string</span></span>  | <span data-ttu-id="81789-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="81789-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="81789-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="81789-134">Request body</span></span>
<span data-ttu-id="81789-135">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="81789-135">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="81789-136">応答</span><span class="sxs-lookup"><span data-stu-id="81789-136">Response</span></span>

<span data-ttu-id="81789-137">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="81789-137">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="81789-138">例 (添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="81789-138">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="81789-139">要求</span><span class="sxs-lookup"><span data-stu-id="81789-139">Request</span></span>
<span data-ttu-id="81789-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="81789-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="81789-141">応答</span><span class="sxs-lookup"><span data-stu-id="81789-141">Response</span></span>
<span data-ttu-id="81789-p104">以下は、応答の例です。注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="81789-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
```


## <a name="example-item-attachment"></a><span data-ttu-id="81789-145">例 (項目の添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="81789-145">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="81789-146">要求</span><span class="sxs-lookup"><span data-stu-id="81789-146">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="81789-147">応答</span><span class="sxs-lookup"><span data-stu-id="81789-147">Response</span></span>
<span data-ttu-id="81789-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="81789-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/eventmessage-post-attachments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
