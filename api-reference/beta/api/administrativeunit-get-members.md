---
title: メンバーを取得します。
description: 管理単位で特定のメンバー (ユーザーまたはグループ) を取得するのにには、この API を使用します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 67067d0e465aab61449a42cd833f9e6ce07fcd12
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526796"
---
# <a name="get-a-member"></a><span data-ttu-id="ae706-103">メンバーを取得します。</span><span class="sxs-lookup"><span data-stu-id="ae706-103">Get a member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae706-104">管理単位で特定のメンバー (ユーザーまたはグループ) を取得するのにには、この API を使用します。</span><span class="sxs-lookup"><span data-stu-id="ae706-104">Use this API to get a specific member (user or group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae706-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ae706-105">Permissions</span></span>
<span data-ttu-id="ae706-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae706-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ae706-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ae706-108">Permission type</span></span>      | <span data-ttu-id="ae706-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ae706-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae706-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ae706-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ae706-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ae706-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ae706-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ae706-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae706-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae706-113">Not supported.</span></span>    |
|<span data-ttu-id="ae706-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae706-114">Application</span></span> | <span data-ttu-id="ae706-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae706-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae706-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ae706-116">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ae706-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae706-117">Request headers</span></span>
| <span data-ttu-id="ae706-118">名前</span><span class="sxs-lookup"><span data-stu-id="ae706-118">Name</span></span>      |<span data-ttu-id="ae706-119">説明</span><span class="sxs-lookup"><span data-stu-id="ae706-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ae706-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae706-120">Authorization</span></span>  | <span data-ttu-id="ae706-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ae706-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae706-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ae706-123">Request body</span></span>
<span data-ttu-id="ae706-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ae706-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae706-125">応答</span><span class="sxs-lookup"><span data-stu-id="ae706-125">Response</span></span>

<span data-ttu-id="ae706-126">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に、[ユーザー](../resources/user.md)または[グループ](../resources/group.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="ae706-126">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) or [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae706-127">例</span><span class="sxs-lookup"><span data-stu-id="ae706-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae706-128">要求</span><span class="sxs-lookup"><span data-stu-id="ae706-128">Request</span></span>
<span data-ttu-id="ae706-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ae706-129">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="ae706-130">応答</span><span class="sxs-lookup"><span data-stu-id="ae706-130">Response</span></span>
<span data-ttu-id="ae706-131">ここでは、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ae706-131">Here is an example of the respone.</span></span> <span data-ttu-id="ae706-132">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="ae706-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ae706-133">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ae706-133">All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "@odata.type":"#microsoft.graph.user",
  "id":"492c5308-59fd-4740-9c83-4b3db07a6d70"
  "accountEnabled":true,
  "businessPhones":[],
  "companyName":null,
  "displayName":"Demo User"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-get-members.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
