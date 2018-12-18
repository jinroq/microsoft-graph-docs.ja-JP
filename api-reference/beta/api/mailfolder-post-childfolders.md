---
title: MailFolder を作成します。
description: 新しい子 mailFolder を作成するのにには、この API を使用します。
author: angelgolfer-ms
ms.openlocfilehash: e893f28878b14fa76d8cda16a5b37f795ed235f2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357275"
---
# <a name="create-mailfolder"></a><span data-ttu-id="f595e-103">MailFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="f595e-103">Create mailFolder</span></span>

> <span data-ttu-id="f595e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f595e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f595e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f595e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f595e-106">新しい子[mailFolder](../resources/mailfolder.md)を作成するのにには、この API を使用します。</span><span class="sxs-lookup"><span data-stu-id="f595e-106">Use this API to create a new child [mailFolder](../resources/mailfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f595e-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f595e-107">Permissions</span></span>

<span data-ttu-id="f595e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f595e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f595e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f595e-110">Permission type</span></span> | <span data-ttu-id="f595e-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f595e-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="f595e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f595e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f595e-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f595e-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f595e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f595e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f595e-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f595e-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f595e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f595e-116">Application</span></span> | <span data-ttu-id="f595e-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f595e-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f595e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f595e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="f595e-119">フォルダー ID の場合、またはよく知られているフォルダー名とクエリの URL では、親フォルダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="f595e-119">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="f595e-120">サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f595e-120">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f595e-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f595e-121">Request headers</span></span>

| <span data-ttu-id="f595e-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f595e-122">Header</span></span> | <span data-ttu-id="f595e-123">値</span><span class="sxs-lookup"><span data-stu-id="f595e-123">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="f595e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f595e-124">Authorization</span></span> | <span data-ttu-id="f595e-125">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="f595e-125"></span></span> <span data-ttu-id="f595e-126">必須です。</span><span class="sxs-lookup"><span data-stu-id="f595e-126">Required.</span></span> |
| <span data-ttu-id="f595e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f595e-127">Content-Type</span></span> | <span data-ttu-id="f595e-128">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="f595e-128"></span></span> <span data-ttu-id="f595e-129">必須です。</span><span class="sxs-lookup"><span data-stu-id="f595e-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f595e-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="f595e-130">Request body</span></span>

<span data-ttu-id="f595e-p106">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。[MailFolder](../resources/mailfolder.md) オブジェクトに対して書き込み可能なプロパティは **displayName** のみです。</span><span class="sxs-lookup"><span data-stu-id="f595e-p106">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="f595e-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f595e-133">Parameter</span></span> | <span data-ttu-id="f595e-134">種類</span><span class="sxs-lookup"><span data-stu-id="f595e-134">Type</span></span> | <span data-ttu-id="f595e-135">説明</span><span class="sxs-lookup"><span data-stu-id="f595e-135">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="f595e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f595e-136">displayName</span></span>|<span data-ttu-id="f595e-137">String</span><span class="sxs-lookup"><span data-stu-id="f595e-137">String</span></span>|<span data-ttu-id="f595e-138">新しいフォルダーの表示名です。</span><span class="sxs-lookup"><span data-stu-id="f595e-138">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="f595e-139">応答</span><span class="sxs-lookup"><span data-stu-id="f595e-139">Response</span></span>

<span data-ttu-id="f595e-140">かどうかは成功すると、このメソッドを返します`201 Created`応答コードおよび応答の本文に[mailFolder](../resources/mailfolder.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f595e-140">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f595e-141">例</span><span class="sxs-lookup"><span data-stu-id="f595e-141">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f595e-142">要求</span><span class="sxs-lookup"><span data-stu-id="f595e-142">Request</span></span>

<span data-ttu-id="f595e-143">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f595e-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_mailfolder"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailFolders/{id}/childFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```

#### <a name="response"></a><span data-ttu-id="f595e-144">応答</span><span class="sxs-lookup"><span data-stu-id="f595e-144">Response</span></span>

<span data-ttu-id="f595e-145">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f595e-145">The following is an example of the response.</span></span>

> <span data-ttu-id="f595e-146">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f595e-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f595e-147">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f595e-147">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
