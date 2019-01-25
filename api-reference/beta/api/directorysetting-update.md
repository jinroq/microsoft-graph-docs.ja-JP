---
title: ディレクトリの設定を更新します。
description: 特定のディレクトリの設定オブジェクトのプロパティを更新します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: baaf6994f7052155173dd58b2c6b021939dc7ba7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529097"
---
# <a name="update-a-directory-setting"></a><span data-ttu-id="50128-103">ディレクトリの設定を更新します。</span><span class="sxs-lookup"><span data-stu-id="50128-103">Update a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50128-104">特定のディレクトリの設定オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="50128-104">Update the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="50128-105">**注**: この API の/beta バージョンは、のみのグループに適用されます。</span><span class="sxs-lookup"><span data-stu-id="50128-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="50128-106">この API の/v1.0 バージョンの名前は*groupSettings を更新*します。</span><span class="sxs-lookup"><span data-stu-id="50128-106">The /v1.0 version of this API has been renamed to *Update groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="50128-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="50128-107">Permissions</span></span>
<span data-ttu-id="50128-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="50128-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50128-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="50128-110">Permission type</span></span>      | <span data-ttu-id="50128-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="50128-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50128-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="50128-112">Delegated (work or school account)</span></span> | <span data-ttu-id="50128-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="50128-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="50128-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="50128-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50128-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50128-115">Not supported.</span></span>    |
|<span data-ttu-id="50128-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="50128-116">Application</span></span> | <span data-ttu-id="50128-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50128-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="50128-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="50128-118">HTTP request</span></span>
<span data-ttu-id="50128-119"><!-- { "blockType": "ignored" } -->テナント全体を更新または、特定の設定をグループ化します。</span><span class="sxs-lookup"><span data-stu-id="50128-119"><!-- { "blockType": "ignored" } --> Update a tenant-wide or group specific setting.</span></span>
```http
PATCH /settings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="50128-120">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="50128-120">Optional request headers</span></span>
| <span data-ttu-id="50128-121">名前</span><span class="sxs-lookup"><span data-stu-id="50128-121">Name</span></span>       | <span data-ttu-id="50128-122">説明</span><span class="sxs-lookup"><span data-stu-id="50128-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="50128-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="50128-123">Authorization</span></span>  | <span data-ttu-id="50128-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="50128-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="50128-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="50128-126">Request body</span></span>
<span data-ttu-id="50128-127">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="50128-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="50128-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50128-128">Property</span></span>     | <span data-ttu-id="50128-129">型</span><span class="sxs-lookup"><span data-stu-id="50128-129">Type</span></span>   |<span data-ttu-id="50128-130">説明</span><span class="sxs-lookup"><span data-stu-id="50128-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="50128-131">values</span><span class="sxs-lookup"><span data-stu-id="50128-131">values</span></span> | <span data-ttu-id="50128-132">settingValue</span><span class="sxs-lookup"><span data-stu-id="50128-132">settingValue</span></span> | <span data-ttu-id="50128-p104">更新された値のセットです。注:コレクション セット全体を指定する必要があります。単一の値のセットを更新することはできません。</span><span class="sxs-lookup"><span data-stu-id="50128-p104">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="50128-136">応答</span><span class="sxs-lookup"><span data-stu-id="50128-136">Response</span></span>

<span data-ttu-id="50128-137">成功した場合、このメソッドは `204 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="50128-137">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="50128-138">例</span><span class="sxs-lookup"><span data-stu-id="50128-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="50128-139">要求</span><span class="sxs-lookup"><span data-stu-id="50128-139">Request</span></span>
<span data-ttu-id="50128-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="50128-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_directorysetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/settings/{id}
Content-type: application/json
Content-length: 178

{
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
##### <a name="response"></a><span data-ttu-id="50128-141">応答</span><span class="sxs-lookup"><span data-stu-id="50128-141">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorysetting"
} -->
```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update directorysetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysetting-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
