---
title: アプリケーションまたはサービス ・ プリンシパルに割り当てられているリストのポリシー
description: アプリケーションまたはサービス ・ プリンシパルに割り当てられているポリシー オブジェクトを取得します。
localization_priority: Normal
ms.openlocfilehash: 417d59228aadd3c6a54c4634416fd577fce11f18
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575962"
---
# <a name="list-policies-assigned-to-application-or-service-principal"></a><span data-ttu-id="6d1bc-103">アプリケーションまたはサービス ・ プリンシパルに割り当てられているリストのポリシー</span><span class="sxs-lookup"><span data-stu-id="6d1bc-103">List Policies assigned to Application or Service Principal</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d1bc-104">アプリケーションまたはサービス ・ プリンシパルに割り当てられている[ポリシー](../resources/policy.md)オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="6d1bc-104">Retrieve the [policy](../resources/policy.md) objects assigned to an application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d1bc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6d1bc-105">Permissions</span></span>
<span data-ttu-id="6d1bc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d1bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d1bc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6d1bc-108">Permission type</span></span>      | <span data-ttu-id="6d1bc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6d1bc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d1bc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6d1bc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6d1bc-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6d1bc-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6d1bc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6d1bc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d1bc-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6d1bc-113">Not supported.</span></span>    |
|<span data-ttu-id="6d1bc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6d1bc-114">Application</span></span> | <span data-ttu-id="6d1bc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6d1bc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d1bc-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6d1bc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/policies
```

> <span data-ttu-id="6d1bc-117">注意: 要求で"id"は、アプリケーションまたはサービス ・ プリンシパル"appid"プロパティではなく"id"プロパティです。</span><span class="sxs-lookup"><span data-stu-id="6d1bc-117">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6d1bc-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6d1bc-118">Request headers</span></span>
| <span data-ttu-id="6d1bc-119">名前</span><span class="sxs-lookup"><span data-stu-id="6d1bc-119">Name</span></span>       | <span data-ttu-id="6d1bc-120">型</span><span class="sxs-lookup"><span data-stu-id="6d1bc-120">Type</span></span> | <span data-ttu-id="6d1bc-121">説明</span><span class="sxs-lookup"><span data-stu-id="6d1bc-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6d1bc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d1bc-122">Authorization</span></span>  | <span data-ttu-id="6d1bc-123">string</span><span class="sxs-lookup"><span data-stu-id="6d1bc-123">string</span></span>  | <span data-ttu-id="6d1bc-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6d1bc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d1bc-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6d1bc-126">Request body</span></span>
<span data-ttu-id="6d1bc-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6d1bc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d1bc-128">応答</span><span class="sxs-lookup"><span data-stu-id="6d1bc-128">Response</span></span>

<span data-ttu-id="6d1bc-129">かどうかは成功すると、このメソッドを返します`200 OK`応答の本体のコードと[ポリシー](../resources/policy.md)オブジェクトを応答します。</span><span class="sxs-lookup"><span data-stu-id="6d1bc-129">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="6d1bc-130">失敗した場合、`4xx`について、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="6d1bc-130">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="6d1bc-131">例</span><span class="sxs-lookup"><span data-stu-id="6d1bc-131">Example</span></span>
<span data-ttu-id="6d1bc-132">次の例では、アプリケーションに割り当てられているポリシーを取得します。</span><span class="sxs-lookup"><span data-stu-id="6d1bc-132">The following example retrieves the policies assigned to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="6d1bc-133">要求</span><span class="sxs-lookup"><span data-stu-id="6d1bc-133">Request</span></span>
<span data-ttu-id="6d1bc-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6d1bc-134">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/applications/{id}/policies
```

##### <a name="response"></a><span data-ttu-id="6d1bc-135">応答</span><span class="sxs-lookup"><span data-stu-id="6d1bc-135">Response</span></span>
<span data-ttu-id="6d1bc-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6d1bc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Cache-Control: private
Content-Type: application/json

{
    "value":[
        {
            "@odata.type":"#microsoft.graph.policy",
            "id":"id-value",
            "alternativeIdentifier":null,
            "definition":["policy-definition"],
            "displayName":"name-value",
            "isOrganizationDefault": true | false,
            "keyCredentials":[key-credentials],
            "type":"type-value"
        }
    ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-list-assigned.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
