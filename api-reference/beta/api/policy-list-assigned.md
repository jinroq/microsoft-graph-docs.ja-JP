---
title: アプリケーションまたはサービス ・ プリンシパルに割り当てられているリストのポリシー
description: アプリケーションまたはサービス ・ プリンシパルに割り当てられているポリシー オブジェクトを取得します。
localization_priority: Normal
ms.openlocfilehash: 1ed39f376b7d090b784f867a59fcb93558bd5f1a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518584"
---
# <a name="list-policies-assigned-to-application-or-service-principal"></a><span data-ttu-id="1d52a-103">アプリケーションまたはサービス ・ プリンシパルに割り当てられているリストのポリシー</span><span class="sxs-lookup"><span data-stu-id="1d52a-103">List Policies assigned to Application or Service Principal</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d52a-104">アプリケーションまたはサービス ・ プリンシパルに割り当てられている[ポリシー](../resources/policy.md)オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="1d52a-104">Retrieve the [policy](../resources/policy.md) objects assigned to an application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d52a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1d52a-105">Permissions</span></span>
<span data-ttu-id="1d52a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1d52a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d52a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1d52a-108">Permission type</span></span>      | <span data-ttu-id="1d52a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1d52a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d52a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1d52a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1d52a-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1d52a-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1d52a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1d52a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d52a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d52a-113">Not supported.</span></span>    |
|<span data-ttu-id="1d52a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1d52a-114">Application</span></span> | <span data-ttu-id="1d52a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d52a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d52a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1d52a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/policies
```

> <span data-ttu-id="1d52a-117">注意: 要求で"id"は、アプリケーションまたはサービス ・ プリンシパル"appid"プロパティではなく"id"プロパティです。</span><span class="sxs-lookup"><span data-stu-id="1d52a-117">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1d52a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d52a-118">Request headers</span></span>
| <span data-ttu-id="1d52a-119">名前</span><span class="sxs-lookup"><span data-stu-id="1d52a-119">Name</span></span>       | <span data-ttu-id="1d52a-120">型</span><span class="sxs-lookup"><span data-stu-id="1d52a-120">Type</span></span> | <span data-ttu-id="1d52a-121">説明</span><span class="sxs-lookup"><span data-stu-id="1d52a-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1d52a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d52a-122">Authorization</span></span>  | <span data-ttu-id="1d52a-123">string</span><span class="sxs-lookup"><span data-stu-id="1d52a-123">string</span></span>  | <span data-ttu-id="1d52a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1d52a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d52a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1d52a-126">Request body</span></span>
<span data-ttu-id="1d52a-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1d52a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d52a-128">応答</span><span class="sxs-lookup"><span data-stu-id="1d52a-128">Response</span></span>

<span data-ttu-id="1d52a-129">かどうかは成功すると、このメソッドを返します`200 OK`応答の本体のコードと[ポリシー](../resources/policy.md)オブジェクトを応答します。</span><span class="sxs-lookup"><span data-stu-id="1d52a-129">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="1d52a-130">失敗した場合、`4xx`について、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="1d52a-130">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="1d52a-131">例</span><span class="sxs-lookup"><span data-stu-id="1d52a-131">Example</span></span>
<span data-ttu-id="1d52a-132">次の例では、アプリケーションに割り当てられているポリシーを取得します。</span><span class="sxs-lookup"><span data-stu-id="1d52a-132">The following example retrieves the policies assigned to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="1d52a-133">要求</span><span class="sxs-lookup"><span data-stu-id="1d52a-133">Request</span></span>
<span data-ttu-id="1d52a-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1d52a-134">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/applications/{id}/policies
```

##### <a name="response"></a><span data-ttu-id="1d52a-135">応答</span><span class="sxs-lookup"><span data-stu-id="1d52a-135">Response</span></span>
<span data-ttu-id="1d52a-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1d52a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
            "isOrganizationDefault":boolean-value,
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
