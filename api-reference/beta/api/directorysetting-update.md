---
title: ディレクトリの設定を更新します。
description: 特定のディレクトリの設定オブジェクトのプロパティを更新します。
author: lleonard-msft
ms.openlocfilehash: c4ff2401397b7a89d30f1513c504acaca5c71140
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308828"
---
# <a name="update-a-directory-setting"></a><span data-ttu-id="0e076-103">ディレクトリの設定を更新します。</span><span class="sxs-lookup"><span data-stu-id="0e076-103">Update a directory setting</span></span>

> <span data-ttu-id="0e076-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0e076-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e076-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0e076-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0e076-106">特定のディレクトリの設定オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0e076-106">Update the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="0e076-107">**注**: この API の/beta バージョンは、のみのグループに適用されます。</span><span class="sxs-lookup"><span data-stu-id="0e076-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="0e076-108">この API の/v1.0 バージョンの名前は*groupSettings を更新*します。</span><span class="sxs-lookup"><span data-stu-id="0e076-108">The /v1.0 version of this API has been renamed to *Update groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e076-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0e076-109">Permissions</span></span>
<span data-ttu-id="0e076-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0e076-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e076-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0e076-112">Permission type</span></span>      | <span data-ttu-id="0e076-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0e076-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e076-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0e076-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0e076-115">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0e076-115">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0e076-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0e076-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e076-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0e076-117">Not supported.</span></span>    |
|<span data-ttu-id="0e076-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0e076-118">Application</span></span> | <span data-ttu-id="0e076-119">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e076-119">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e076-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0e076-120">HTTP request</span></span>
<span data-ttu-id="0e076-121"><!-- { "blockType": "ignored" } -->テナント全体を更新または、特定の設定をグループ化します。</span><span class="sxs-lookup"><span data-stu-id="0e076-121"><!-- { "blockType": "ignored" } --> Update a tenant-wide or group specific setting.</span></span>
```http
PATCH /settings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="0e076-122">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0e076-122">Optional request headers</span></span>
| <span data-ttu-id="0e076-123">名前</span><span class="sxs-lookup"><span data-stu-id="0e076-123">Name</span></span>       | <span data-ttu-id="0e076-124">説明</span><span class="sxs-lookup"><span data-stu-id="0e076-124">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0e076-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e076-125">Authorization</span></span>  | <span data-ttu-id="0e076-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0e076-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e076-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="0e076-128">Request body</span></span>
<span data-ttu-id="0e076-129">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="0e076-129">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="0e076-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e076-130">Property</span></span>     | <span data-ttu-id="0e076-131">種類</span><span class="sxs-lookup"><span data-stu-id="0e076-131">Type</span></span>   |<span data-ttu-id="0e076-132">説明</span><span class="sxs-lookup"><span data-stu-id="0e076-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0e076-133">values</span><span class="sxs-lookup"><span data-stu-id="0e076-133">values</span></span> | <span data-ttu-id="0e076-134">settingValue</span><span class="sxs-lookup"><span data-stu-id="0e076-134">settingValue</span></span> | <span data-ttu-id="0e076-p105">更新された値のセットです。注:コレクション セット全体を指定する必要があります。単一の値のセットを更新することはできません。</span><span class="sxs-lookup"><span data-stu-id="0e076-p105">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="0e076-138">応答</span><span class="sxs-lookup"><span data-stu-id="0e076-138">Response</span></span>

<span data-ttu-id="0e076-139">成功した場合、このメソッドは `204 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="0e076-139">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0e076-140">例</span><span class="sxs-lookup"><span data-stu-id="0e076-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0e076-141">要求</span><span class="sxs-lookup"><span data-stu-id="0e076-141">Request</span></span>
<span data-ttu-id="0e076-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0e076-142">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="0e076-143">応答</span><span class="sxs-lookup"><span data-stu-id="0e076-143">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update directorysetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->