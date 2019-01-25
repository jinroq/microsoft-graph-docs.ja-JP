---
title: 'section: copyToSectionGroup'
description: 特定のセクション グループにセクションをコピーします。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 0b67f140871b6fa81c81f3e5ffceee492b62b3af
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514167"
---
# <a name="section-copytosectiongroup"></a><span data-ttu-id="3bb80-103">section: copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="3bb80-103">section: copyToSectionGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bb80-104">特定のセクション グループにセクションをコピーします。</span><span class="sxs-lookup"><span data-stu-id="3bb80-104">Copies a section to a specific section group.</span></span>

<span data-ttu-id="3bb80-105">Copy 操作では、非同期の呼び出しパターンに従います。まず Copy 操作を呼び出し、次に結果の操作エンドポイントをポーリングします。</span><span class="sxs-lookup"><span data-stu-id="3bb80-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="3bb80-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3bb80-106">Permissions</span></span>
<span data-ttu-id="3bb80-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3bb80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bb80-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3bb80-109">Permission type</span></span>      | <span data-ttu-id="3bb80-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3bb80-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3bb80-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3bb80-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3bb80-112">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bb80-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="3bb80-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3bb80-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3bb80-114">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3bb80-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="3bb80-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3bb80-115">Application</span></span> | <span data-ttu-id="3bb80-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bb80-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3bb80-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3bb80-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
POST /sites/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="3bb80-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3bb80-118">Request headers</span></span>
| <span data-ttu-id="3bb80-119">名前</span><span class="sxs-lookup"><span data-stu-id="3bb80-119">Name</span></span>       | <span data-ttu-id="3bb80-120">型</span><span class="sxs-lookup"><span data-stu-id="3bb80-120">Type</span></span> | <span data-ttu-id="3bb80-121">説明</span><span class="sxs-lookup"><span data-stu-id="3bb80-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3bb80-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3bb80-122">Authorization</span></span>  | <span data-ttu-id="3bb80-123">string</span><span class="sxs-lookup"><span data-stu-id="3bb80-123">string</span></span>  | <span data-ttu-id="3bb80-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3bb80-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3bb80-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3bb80-126">Content-Type</span></span> | <span data-ttu-id="3bb80-127">string</span><span class="sxs-lookup"><span data-stu-id="3bb80-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="3bb80-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="3bb80-128">Request body</span></span>
<span data-ttu-id="3bb80-129">要求本文では、操作に必要なパラメーターを格納する JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="3bb80-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="3bb80-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="3bb80-130">Parameter</span></span>    | <span data-ttu-id="3bb80-131">型</span><span class="sxs-lookup"><span data-stu-id="3bb80-131">Type</span></span>   |<span data-ttu-id="3bb80-132">説明</span><span class="sxs-lookup"><span data-stu-id="3bb80-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3bb80-133">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="3bb80-133">siteCollectionId</span></span>|<span data-ttu-id="3bb80-134">String</span><span class="sxs-lookup"><span data-stu-id="3bb80-134">String</span></span>|<span data-ttu-id="3bb80-135">コピーする SharePoint サイトの id です。</span><span class="sxs-lookup"><span data-stu-id="3bb80-135">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="3bb80-136">Office 365 チーム サイトにコピーするときにのみを使用します。</span><span class="sxs-lookup"><span data-stu-id="3bb80-136">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="3bb80-137">siteId</span><span class="sxs-lookup"><span data-stu-id="3bb80-137">siteId</span></span>|<span data-ttu-id="3bb80-138">String</span><span class="sxs-lookup"><span data-stu-id="3bb80-138">String</span></span>|<span data-ttu-id="3bb80-139">コピーする SharePoint web の id です。</span><span class="sxs-lookup"><span data-stu-id="3bb80-139">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="3bb80-140">Office 365 チーム サイトにコピーするときにのみを使用します。</span><span class="sxs-lookup"><span data-stu-id="3bb80-140">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="3bb80-141">groupId</span><span class="sxs-lookup"><span data-stu-id="3bb80-141">groupId</span></span>|<span data-ttu-id="3bb80-142">文字列</span><span class="sxs-lookup"><span data-stu-id="3bb80-142">String</span></span>|<span data-ttu-id="3bb80-p105">コピー先グループの ID。Office 365 グループにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="3bb80-p105">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="3bb80-145">id</span><span class="sxs-lookup"><span data-stu-id="3bb80-145">id</span></span>|<span data-ttu-id="3bb80-146">String</span><span class="sxs-lookup"><span data-stu-id="3bb80-146">String</span></span>|<span data-ttu-id="3bb80-p106">必須。目的のセクション グループの ID。</span><span class="sxs-lookup"><span data-stu-id="3bb80-p106">Required. The id of the destination section group.</span></span> |
|<span data-ttu-id="3bb80-149">renameAs</span><span class="sxs-lookup"><span data-stu-id="3bb80-149">renameAs</span></span>|<span data-ttu-id="3bb80-150">String</span><span class="sxs-lookup"><span data-stu-id="3bb80-150">String</span></span>|<span data-ttu-id="3bb80-p107">コピーの名前。既定値は、既存のアイテムの名前になります。</span><span class="sxs-lookup"><span data-stu-id="3bb80-p107">The name of the copy. Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="3bb80-153">応答</span><span class="sxs-lookup"><span data-stu-id="3bb80-153">Response</span></span>

<span data-ttu-id="3bb80-p108">成功した場合、このメソッドは `202 Accepted` 応答コードと `Operation-Location` ヘッダーを返します。Operation-Location エンドポイントをポーリングして、[コピー操作の状態を取得します](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="3bb80-p108">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="3bb80-156">例</span><span class="sxs-lookup"><span data-stu-id="3bb80-156">Example</span></span>
<span data-ttu-id="3bb80-157">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="3bb80-157">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3bb80-158">要求</span><span class="sxs-lookup"><span data-stu-id="3bb80-158">Request</span></span>
<span data-ttu-id="3bb80-159">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3bb80-159">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytosectiongroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sections/{id}/copyToSectionGroup
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="3bb80-160">応答</span><span class="sxs-lookup"><span data-stu-id="3bb80-160">Response</span></span>
<span data-ttu-id="3bb80-161">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="3bb80-161">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "section: copyToSectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/section-copytosectiongroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
