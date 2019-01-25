---
title: MailSearchFolder を更新します。
description: MailSearchFolder オブジェクトの書き込み可能なプロパティを更新します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 54e901751fc404ba2099205c6b16d86c99d9b05f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528467"
---
# <a name="update-mailsearchfolder"></a><span data-ttu-id="9d356-103">MailSearchFolder を更新します。</span><span class="sxs-lookup"><span data-stu-id="9d356-103">Update mailSearchFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d356-104">[MailSearchFolder](../resources/mailsearchfolder.md)オブジェクトの書き込み可能なプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9d356-104">Update the writable properties of [mailSearchFolder](../resources/mailsearchfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d356-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9d356-105">Permissions</span></span>
<span data-ttu-id="9d356-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9d356-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d356-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9d356-108">Permission type</span></span>      | <span data-ttu-id="9d356-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9d356-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d356-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9d356-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9d356-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d356-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9d356-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9d356-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d356-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d356-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9d356-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9d356-114">Application</span></span> | <span data-ttu-id="9d356-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d356-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d356-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9d356-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9d356-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9d356-117">Request headers</span></span>
| <span data-ttu-id="9d356-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9d356-118">Header</span></span>       | <span data-ttu-id="9d356-119">値</span><span class="sxs-lookup"><span data-stu-id="9d356-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9d356-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d356-120">Authorization</span></span>  | <span data-ttu-id="9d356-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9d356-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9d356-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9d356-123">Content-Type</span></span>  | <span data-ttu-id="9d356-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9d356-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9d356-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9d356-126">Request body</span></span>
<span data-ttu-id="9d356-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="9d356-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9d356-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9d356-130">Property</span></span>     | <span data-ttu-id="9d356-131">型</span><span class="sxs-lookup"><span data-stu-id="9d356-131">Type</span></span>   |<span data-ttu-id="9d356-132">説明</span><span class="sxs-lookup"><span data-stu-id="9d356-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9d356-133">displayName</span><span class="sxs-lookup"><span data-stu-id="9d356-133">displayName</span></span> | <span data-ttu-id="9d356-134">String</span><span class="sxs-lookup"><span data-stu-id="9d356-134">String</span></span> | <span data-ttu-id="9d356-135">[MailFolder](../resources/mailfolder.md)の表示名です。</span><span class="sxs-lookup"><span data-stu-id="9d356-135">The display name of the [mailFolder](../resources/mailfolder.md).</span></span>|
| <span data-ttu-id="9d356-136">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="9d356-136">includeNestedFolders</span></span> | <span data-ttu-id="9d356-137">ブール値</span><span class="sxs-lookup"><span data-stu-id="9d356-137">Boolean</span></span> | <span data-ttu-id="9d356-138">どのメールボックス フォルダー階層を走査する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d356-138">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="9d356-139">`true`詳細検索をする必要があることを意味時に`false`簡易検索を代わりに行う必要があることを意味します。</span><span class="sxs-lookup"><span data-stu-id="9d356-139">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="9d356-140">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="9d356-140">sourceFolderIDs</span></span> | <span data-ttu-id="9d356-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9d356-141">String collection</span></span> | <span data-ttu-id="9d356-142">メールボックス フォルダーをマイニングする必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d356-142">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="9d356-143">filterQuery</span><span class="sxs-lookup"><span data-stu-id="9d356-143">filterQuery</span></span> | <span data-ttu-id="9d356-144">String</span><span class="sxs-lookup"><span data-stu-id="9d356-144">String</span></span> | <span data-ttu-id="9d356-145">メッセージをフィルタ リングする OData クエリです。</span><span class="sxs-lookup"><span data-stu-id="9d356-145">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="9d356-146">応答</span><span class="sxs-lookup"><span data-stu-id="9d356-146">Response</span></span>
<span data-ttu-id="9d356-147">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [mailFolder](../resources/mailfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9d356-147">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d356-148">例</span><span class="sxs-lookup"><span data-stu-id="9d356-148">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9d356-149">要求</span><span class="sxs-lookup"><span data-stu-id="9d356-149">Request</span></span>
<span data-ttu-id="9d356-150">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9d356-150">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_mailsearchfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
Content-type: application/json
Content-length: 159

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "filterQuery": "contains(subject, 'Analytics')))"
}
```

#### <a name="response"></a><span data-ttu-id="9d356-151">応答</span><span class="sxs-lookup"><span data-stu-id="9d356-151">Response</span></span>
<span data-ttu-id="9d356-152">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9d356-152">The following is an example of the response.</span></span>
><span data-ttu-id="9d356-153">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="9d356-153">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9d356-154">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9d356-154">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.mailSearchFolder",
  "id": "AAMkAGVmMDEzMx",
  "displayName": "Get MyAnalytics",
  "parentFolderId": "AAMkAGVmMDEzMy",
  "childFolderCount": 0,
  "unreadItemCount": 0,
  "totalItemCount": 0,
  "wellKnownName": null,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIDs": [
      "AAMkAGVmMDEzMi"
  ],
  "filterQuery": "contains(subject, 'Analytics')"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update mailSearchFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailsearchfolder-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
