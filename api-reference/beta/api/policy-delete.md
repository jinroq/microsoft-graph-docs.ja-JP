---
title: ポリシーの削除
description: ポリシーを削除します。
localization_priority: Normal
ms.openlocfilehash: 6467259fc0cca067deb25bc561ddf18f54760e92
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337461"
---
# <a name="delete-policy"></a><span data-ttu-id="17f20-103">ポリシーの削除</span><span class="sxs-lookup"><span data-stu-id="17f20-103">Delete Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17f20-104">[ポリシー](../resources/policy.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="17f20-104">Delete a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="17f20-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="17f20-105">Permissions</span></span>
<span data-ttu-id="17f20-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="17f20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17f20-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="17f20-108">Permission type</span></span>      | <span data-ttu-id="17f20-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="17f20-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17f20-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="17f20-110">Delegated (work or school account)</span></span> | <span data-ttu-id="17f20-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="17f20-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="17f20-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="17f20-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17f20-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="17f20-113">Not supported.</span></span>    |
|<span data-ttu-id="17f20-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="17f20-114">Application</span></span> | <span data-ttu-id="17f20-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="17f20-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="17f20-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="17f20-116">HTTP request</span></span>

```http
DELETE /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="17f20-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="17f20-117">Request headers</span></span>
| <span data-ttu-id="17f20-118">名前</span><span class="sxs-lookup"><span data-stu-id="17f20-118">Name</span></span>       | <span data-ttu-id="17f20-119">型</span><span class="sxs-lookup"><span data-stu-id="17f20-119">Type</span></span> | <span data-ttu-id="17f20-120">説明</span><span class="sxs-lookup"><span data-stu-id="17f20-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="17f20-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="17f20-121">Authorization</span></span>  | <span data-ttu-id="17f20-122">string</span><span class="sxs-lookup"><span data-stu-id="17f20-122">string</span></span>  | <span data-ttu-id="17f20-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="17f20-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17f20-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="17f20-125">Request body</span></span>
<span data-ttu-id="17f20-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="17f20-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17f20-127">応答</span><span class="sxs-lookup"><span data-stu-id="17f20-127">Response</span></span>

<span data-ttu-id="17f20-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="17f20-128">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="17f20-129">失敗した場合...</span><span class="sxs-lookup"><span data-stu-id="17f20-129">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="17f20-130">例</span><span class="sxs-lookup"><span data-stu-id="17f20-130">Example</span></span>
<span data-ttu-id="17f20-131">次の例では、ポリシーを削除します。</span><span class="sxs-lookup"><span data-stu-id="17f20-131">The following example deletes a policy.</span></span>

##### <a name="request"></a><span data-ttu-id="17f20-132">要求</span><span class="sxs-lookup"><span data-stu-id="17f20-132">Request</span></span>
<span data-ttu-id="17f20-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="17f20-133">Here is an example of the request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="17f20-134">応答</span><span class="sxs-lookup"><span data-stu-id="17f20-134">Response</span></span>
<span data-ttu-id="17f20-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="17f20-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
