---
title: ドメインを削除する
description: テナントからドメインを削除します。
author: lleonard-msft
ms.openlocfilehash: eeebfb0c4c654dbfc119b4af97ccab6e27fbef91
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353054"
---
# <a name="delete-domain"></a><span data-ttu-id="214ac-103">ドメインを削除する</span><span class="sxs-lookup"><span data-stu-id="214ac-103">Delete domain</span></span>

<span data-ttu-id="214ac-104">テナントからドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="214ac-104">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="214ac-105">**重要:**</span><span class="sxs-lookup"><span data-stu-id="214ac-105">**Important:**</span></span>
> - <span data-ttu-id="214ac-106">削除されたドメインは回復できません。</span><span class="sxs-lookup"><span data-stu-id="214ac-106">Deleted domains are not recoverable.</span></span><br />
> - <span data-ttu-id="214ac-p101">ドメインにまだ依存しているリソースまたはオブジェクトがある場合、削除の試行は失敗します。[List domainNameReferences](domain-list-domainnamereferences.md) API を使用して、すべての依存リソースを探すことができます。</span><span class="sxs-lookup"><span data-stu-id="214ac-p101">Attempts to delete will fail if there are any resources or objects still dependent on the domain. You can find all dependent resources by using the [List domainNameReferences](domain-list-domainnamereferences.md) API.</span></span>

## <a name="permissions"></a><span data-ttu-id="214ac-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="214ac-109">Permissions</span></span>

<span data-ttu-id="214ac-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="214ac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="214ac-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="214ac-112">Permission type</span></span>      | <span data-ttu-id="214ac-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="214ac-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="214ac-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="214ac-114">Delegated (work or school account)</span></span> | <span data-ttu-id="214ac-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="214ac-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="214ac-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="214ac-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="214ac-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="214ac-117">Not supported.</span></span>    |
|<span data-ttu-id="214ac-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="214ac-118">Application</span></span> | <span data-ttu-id="214ac-119">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="214ac-119">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="214ac-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="214ac-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="214ac-121">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="214ac-121">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="214ac-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="214ac-122">Request headers</span></span>

| <span data-ttu-id="214ac-123">名前</span><span class="sxs-lookup"><span data-stu-id="214ac-123">Name</span></span>       | <span data-ttu-id="214ac-124">説明</span><span class="sxs-lookup"><span data-stu-id="214ac-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="214ac-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="214ac-125">Authorization</span></span>  | <span data-ttu-id="214ac-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="214ac-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="214ac-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="214ac-128">Content-Type</span></span>  | <span data-ttu-id="214ac-129">application/json</span><span class="sxs-lookup"><span data-stu-id="214ac-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="214ac-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="214ac-130">Request body</span></span>

<span data-ttu-id="214ac-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="214ac-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="214ac-132">応答</span><span class="sxs-lookup"><span data-stu-id="214ac-132">Response</span></span>

<span data-ttu-id="214ac-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文は返されません。</span><span class="sxs-lookup"><span data-stu-id="214ac-p104">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="214ac-135">例</span><span class="sxs-lookup"><span data-stu-id="214ac-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="214ac-136">要求</span><span class="sxs-lookup"><span data-stu-id="214ac-136">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/domains/contoso.com
```

##### <a name="response"></a><span data-ttu-id="214ac-137">応答</span><span class="sxs-lookup"><span data-stu-id="214ac-137">Response</span></span>

<span data-ttu-id="214ac-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="214ac-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->