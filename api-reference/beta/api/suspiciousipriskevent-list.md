---
title: リスト suspiciousIpRiskEvents
description: suspiciousipriskevent オブジェクトのリストを取得します。
localization_priority: Normal
ms.openlocfilehash: 1caad773d401367b93bece5d30191a5c98b7b935
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537171"
---
# <a name="list-suspiciousipriskevents"></a><span data-ttu-id="0b257-103">リスト suspiciousIpRiskEvents</span><span class="sxs-lookup"><span data-stu-id="0b257-103">List suspiciousIpRiskEvents</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b257-104">suspiciousipriskevent オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="0b257-104">Retrieve a list of suspiciousipriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="0b257-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0b257-105">Permissions</span></span>
<span data-ttu-id="0b257-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0b257-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b257-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0b257-108">Permission type</span></span>      | <span data-ttu-id="0b257-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0b257-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b257-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0b257-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0b257-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b257-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="0b257-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0b257-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b257-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0b257-113">Not supported.</span></span>    |
|<span data-ttu-id="0b257-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0b257-114">Application</span></span> | <span data-ttu-id="0b257-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b257-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b257-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0b257-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /suspiciousIpRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="0b257-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0b257-117">Request headers</span></span>
| <span data-ttu-id="0b257-118">名前</span><span class="sxs-lookup"><span data-stu-id="0b257-118">Name</span></span>      |<span data-ttu-id="0b257-119">説明</span><span class="sxs-lookup"><span data-stu-id="0b257-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0b257-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b257-120">Authorization</span></span>  | <span data-ttu-id="0b257-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0b257-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0b257-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0b257-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="0b257-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="0b257-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b257-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0b257-126">Request body</span></span>
<span data-ttu-id="0b257-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0b257-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b257-128">応答</span><span class="sxs-lookup"><span data-stu-id="0b257-128">Response</span></span>

<span data-ttu-id="0b257-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="0b257-129">If successful, this method returns a `200 OK` response code and collection of [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0b257-130">例</span><span class="sxs-lookup"><span data-stu-id="0b257-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0b257-131">要求</span><span class="sxs-lookup"><span data-stu-id="0b257-131">Request</span></span>
<span data-ttu-id="0b257-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0b257-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_suspiciousipriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/suspiciousIpRiskEvents
```
##### <a name="response"></a><span data-ttu-id="0b257-133">応答</span><span class="sxs-lookup"><span data-stu-id="0b257-133">Response</span></span>
<span data-ttu-id="0b257-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0b257-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.suspiciousIpRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 290

{
  "value": [
    {
      "closedDateTime": null,
      "createdDateTime": "2016-02-03T06:08:35.123512Z",
      "id": "02e8bfd1-5231-1006-01cc-434f84e0859e-97b7301f-bc05-8e2c-fdfa-2004eb66ff70-287e7b9b-1d60-aa96-6ddb-65c81ee31475",
      "ipAddress": "95.31.18.119",
      "location": "Moskva, Russia, RU",
      "riskEventDateTime": "2016-02-03T05:33:49.9516789Z",
      "riskEventStatus": "active",
      "riskLevel": "low",
      "riskType": "SuspiciousIpRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "97b7301f-bc05-8e2c-fdfa-2004eb66ff70",
      "userPrincipalName": "jon@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List suspiciousIpRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/suspiciousipriskevent-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
