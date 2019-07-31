---
title: メンバーを取得する
description: この API を使用して、管理単位で特定のメンバー (ユーザーまたはグループ) を取得します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 81a1165148dbaa81740cdc4d7b9dbf65f7d8cd4b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945859"
---
# <a name="get-a-member"></a><span data-ttu-id="f375e-103">メンバーを取得する</span><span class="sxs-lookup"><span data-stu-id="f375e-103">Get a member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f375e-104">この API を使用して、管理単位で特定のメンバー (ユーザーまたはグループ) を取得します。</span><span class="sxs-lookup"><span data-stu-id="f375e-104">Use this API to get a specific member (user or group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="f375e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f375e-105">Permissions</span></span>
<span data-ttu-id="f375e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f375e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f375e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f375e-108">Permission type</span></span>      | <span data-ttu-id="f375e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f375e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f375e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f375e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f375e-111">AdministrativeUnit、AdministrativeUnit、Directory.accessasuser.all、および all のいずれかを取得します。すべてのディレクトリは、です。</span><span class="sxs-lookup"><span data-stu-id="f375e-111">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f375e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f375e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f375e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f375e-113">Not supported.</span></span>    |
|<span data-ttu-id="f375e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f375e-114">Application</span></span> | <span data-ttu-id="f375e-115">AdministrativeUnit。すべて、AdministrativeUnit、およびすべてのディレクトリを読み取ることができます。すべての</span><span class="sxs-lookup"><span data-stu-id="f375e-115">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f375e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f375e-116">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f375e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f375e-117">Request headers</span></span>
| <span data-ttu-id="f375e-118">名前</span><span class="sxs-lookup"><span data-stu-id="f375e-118">Name</span></span>      |<span data-ttu-id="f375e-119">説明</span><span class="sxs-lookup"><span data-stu-id="f375e-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f375e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f375e-120">Authorization</span></span>  | <span data-ttu-id="f375e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f375e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f375e-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="f375e-123">Request body</span></span>
<span data-ttu-id="f375e-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f375e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f375e-125">応答</span><span class="sxs-lookup"><span data-stu-id="f375e-125">Response</span></span>

<span data-ttu-id="f375e-126">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[ユーザー](../resources/user.md)または[グループ](../resources/group.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f375e-126">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) or [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f375e-127">例</span><span class="sxs-lookup"><span data-stu-id="f375e-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f375e-128">要求</span><span class="sxs-lookup"><span data-stu-id="f375e-128">Request</span></span>
<span data-ttu-id="f375e-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f375e-129">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="f375e-130">応答</span><span class="sxs-lookup"><span data-stu-id="f375e-130">Response</span></span>
<span data-ttu-id="f375e-131">次に、その一例を示します。</span><span class="sxs-lookup"><span data-stu-id="f375e-131">Here is an example of the respone.</span></span> <span data-ttu-id="f375e-132">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="f375e-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f375e-133">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f375e-133">All of the properties will be returned from an actual call.</span></span>

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
