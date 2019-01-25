---
title: IdentityProvider を削除します。
description: 既存の identityProvider を削除します。
localization_priority: Normal
ms.openlocfilehash: bb64f10b656697ab2cf611dd9be0468c295b15e8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514356"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="c76d7-103">IdentityProvider を削除します。</span><span class="sxs-lookup"><span data-stu-id="c76d7-103">Delete identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c76d7-104">既存の[identityProvider](../resources/identityprovider.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="c76d7-104">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c76d7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c76d7-105">Permissions</span></span>

<span data-ttu-id="c76d7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c76d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c76d7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c76d7-108">Permission type</span></span>      | <span data-ttu-id="c76d7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c76d7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c76d7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c76d7-110">Delegated (work or school account)</span></span>|<span data-ttu-id="c76d7-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c76d7-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="c76d7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c76d7-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c76d7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c76d7-113">Not supported.</span></span>|
|<span data-ttu-id="c76d7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c76d7-114">Application</span></span>|<span data-ttu-id="c76d7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c76d7-115">Not supported.</span></span>|

<span data-ttu-id="c76d7-116">職場または学校のアカウントは、テナントのグローバル ・ アドミニストレーターである必要があります。</span><span class="sxs-lookup"><span data-stu-id="c76d7-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="c76d7-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c76d7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c76d7-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c76d7-118">Request headers</span></span>

|<span data-ttu-id="c76d7-119">名前</span><span class="sxs-lookup"><span data-stu-id="c76d7-119">Name</span></span>|<span data-ttu-id="c76d7-120">説明</span><span class="sxs-lookup"><span data-stu-id="c76d7-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="c76d7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c76d7-121">Authorization</span></span>|<span data-ttu-id="c76d7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c76d7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c76d7-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="c76d7-124">Request body</span></span>

<span data-ttu-id="c76d7-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c76d7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c76d7-126">応答</span><span class="sxs-lookup"><span data-stu-id="c76d7-126">Response</span></span>

<span data-ttu-id="c76d7-127">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="c76d7-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c76d7-128">例</span><span class="sxs-lookup"><span data-stu-id="c76d7-128">Example</span></span>

<span data-ttu-id="c76d7-129">次の使用例は、 **identityProvider**を削除します。</span><span class="sxs-lookup"><span data-stu-id="c76d7-129">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="c76d7-130">要求</span><span class="sxs-lookup"><span data-stu-id="c76d7-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="c76d7-131">応答</span><span class="sxs-lookup"><span data-stu-id="c76d7-131">Response</span></span>

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
  "description": "Delete identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/identityprovider-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
