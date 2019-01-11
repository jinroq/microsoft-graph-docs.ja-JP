---
title: ディレクトリの設定を削除します。
description: ディレクトリの設定を削除します。
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 35954404b21eea883c9240bb1647feb85f490b16
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843828"
---
# <a name="delete-a-directory-setting"></a><span data-ttu-id="be0a3-103">ディレクトリの設定を削除します。</span><span class="sxs-lookup"><span data-stu-id="be0a3-103">Delete a directory setting</span></span>

> <span data-ttu-id="be0a3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="be0a3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be0a3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be0a3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="be0a3-106">ディレクトリの設定を削除します。</span><span class="sxs-lookup"><span data-stu-id="be0a3-106">Delete a directory setting.</span></span>

> <span data-ttu-id="be0a3-107">**注**: この API の/beta バージョンは、のみのグループに適用されます。</span><span class="sxs-lookup"><span data-stu-id="be0a3-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="be0a3-108">この API の/v1.0 バージョンは、 *groupSettings を削除*するのには名前が変更されましたが。</span><span class="sxs-lookup"><span data-stu-id="be0a3-108">The /v1.0 version of this API has been renamed to *Delete groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="be0a3-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="be0a3-109">Permissions</span></span>
<span data-ttu-id="be0a3-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be0a3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be0a3-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="be0a3-112">Permission type</span></span>      | <span data-ttu-id="be0a3-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="be0a3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be0a3-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="be0a3-114">Delegated (work or school account)</span></span> | <span data-ttu-id="be0a3-115">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="be0a3-115">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="be0a3-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="be0a3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be0a3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be0a3-117">Not supported.</span></span>    |
|<span data-ttu-id="be0a3-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="be0a3-118">Application</span></span> | <span data-ttu-id="be0a3-119">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be0a3-119">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="be0a3-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="be0a3-120">HTTP request</span></span>
<span data-ttu-id="be0a3-121"><!-- { "blockType": "ignored" } -->特定のテナント全体を削除するか、グループの設定</span><span class="sxs-lookup"><span data-stu-id="be0a3-121"><!-- { "blockType": "ignored" } --> Delete a specific tenant-wide or group setting</span></span>
```http
DELETE /settings/{id}
DELETE /groups/{id}/settings/{id}

```
## <a name="request-headers"></a><span data-ttu-id="be0a3-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="be0a3-122">Request headers</span></span>
| <span data-ttu-id="be0a3-123">名前</span><span class="sxs-lookup"><span data-stu-id="be0a3-123">Name</span></span>       | <span data-ttu-id="be0a3-124">説明</span><span class="sxs-lookup"><span data-stu-id="be0a3-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="be0a3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="be0a3-125">Authorization</span></span>  | <span data-ttu-id="be0a3-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="be0a3-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be0a3-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="be0a3-128">Request body</span></span>
<span data-ttu-id="be0a3-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="be0a3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be0a3-130">応答</span><span class="sxs-lookup"><span data-stu-id="be0a3-130">Response</span></span>

<span data-ttu-id="be0a3-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="be0a3-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be0a3-133">例</span><span class="sxs-lookup"><span data-stu-id="be0a3-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be0a3-134">要求</span><span class="sxs-lookup"><span data-stu-id="be0a3-134">Request</span></span>
<span data-ttu-id="be0a3-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="be0a3-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directorysetting"
}-->
```http
DELETE https://graph.microsoft.com/beta/settings/{id}
```
##### <a name="response"></a><span data-ttu-id="be0a3-136">応答</span><span class="sxs-lookup"><span data-stu-id="be0a3-136">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
