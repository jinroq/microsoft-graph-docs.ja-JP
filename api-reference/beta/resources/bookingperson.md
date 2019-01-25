---
title: bookingPerson リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: be00e59e2378c454cd9c939f992376dd9c54c3b0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508406"
---
# <a name="bookingperson-resource-type"></a><span data-ttu-id="94521-104">bookingPerson リソースの種類</span><span class="sxs-lookup"><span data-stu-id="94521-104">bookingPerson resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="94521-105">これは、 [bookingCustomer](bookingcustomer.md)または[bookingStaffMember](bookingstaffmember.md)であることができます、Microsoft の予約のビジネス ユーザーの基本型です。</span><span class="sxs-lookup"><span data-stu-id="94521-105">This is a base type for a person in a Microsoft Bookings business, which can be a [bookingCustomer](bookingcustomer.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="94521-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="94521-106">Properties</span></span>
| <span data-ttu-id="94521-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="94521-107">Property</span></span>     | <span data-ttu-id="94521-108">型</span><span class="sxs-lookup"><span data-stu-id="94521-108">Type</span></span>   |<span data-ttu-id="94521-109">説明</span><span class="sxs-lookup"><span data-stu-id="94521-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94521-110">displayName</span><span class="sxs-lookup"><span data-stu-id="94521-110">displayName</span></span>|<span data-ttu-id="94521-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="94521-111">String</span></span>|<span data-ttu-id="94521-112">派生のエンティティは、顧客とのインターフェイスの名前です。</span><span class="sxs-lookup"><span data-stu-id="94521-112">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="94521-113">emailAddress</span><span class="sxs-lookup"><span data-stu-id="94521-113">emailAddress</span></span>|<span data-ttu-id="94521-114">String</span><span class="sxs-lookup"><span data-stu-id="94521-114">String</span></span>|<span data-ttu-id="94521-115">ユーザーの電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="94521-115">The email address of the person.</span></span>|
|<span data-ttu-id="94521-116">id</span><span class="sxs-lookup"><span data-stu-id="94521-116">id</span></span>|<span data-ttu-id="94521-117">文字列</span><span class="sxs-lookup"><span data-stu-id="94521-117">String</span></span>| <span data-ttu-id="94521-118">派生エンティティの ID です。</span><span class="sxs-lookup"><span data-stu-id="94521-118">The ID for the derived entity.</span></span> <span data-ttu-id="94521-119">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="94521-119">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94521-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="94521-120">Relationships</span></span>
<span data-ttu-id="94521-121">なし</span><span class="sxs-lookup"><span data-stu-id="94521-121">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="94521-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="94521-122">JSON representation</span></span>

<span data-ttu-id="94521-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="94521-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingPerson"
}-->

```json
{
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingPerson resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingperson.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
