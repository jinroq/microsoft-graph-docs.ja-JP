---
title: bookingperson リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: be00e59e2378c454cd9c939f992376dd9c54c3b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543803"
---
# <a name="bookingperson-resource-type"></a><span data-ttu-id="0cf74-104">bookingperson リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0cf74-104">bookingPerson resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="0cf74-105">これは、Microsoft の予約ビジネスにおける個人の基本型です。これは、 [bookingcustomer](bookingcustomer.md)または[bookingStaffMember](bookingstaffmember.md)にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0cf74-105">This is a base type for a person in a Microsoft Bookings business, which can be a [bookingCustomer](bookingcustomer.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0cf74-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0cf74-106">Properties</span></span>
| <span data-ttu-id="0cf74-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0cf74-107">Property</span></span>     | <span data-ttu-id="0cf74-108">型</span><span class="sxs-lookup"><span data-stu-id="0cf74-108">Type</span></span>   |<span data-ttu-id="0cf74-109">説明</span><span class="sxs-lookup"><span data-stu-id="0cf74-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0cf74-110">displayName</span><span class="sxs-lookup"><span data-stu-id="0cf74-110">displayName</span></span>|<span data-ttu-id="0cf74-111">String</span><span class="sxs-lookup"><span data-stu-id="0cf74-111">String</span></span>|<span data-ttu-id="0cf74-112">顧客とのインターフェイスとなる派生エンティティの名前。</span><span class="sxs-lookup"><span data-stu-id="0cf74-112">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="0cf74-113">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0cf74-113">emailAddress</span></span>|<span data-ttu-id="0cf74-114">String</span><span class="sxs-lookup"><span data-stu-id="0cf74-114">String</span></span>|<span data-ttu-id="0cf74-115">個人の電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="0cf74-115">The email address of the person.</span></span>|
|<span data-ttu-id="0cf74-116">id</span><span class="sxs-lookup"><span data-stu-id="0cf74-116">id</span></span>|<span data-ttu-id="0cf74-117">String</span><span class="sxs-lookup"><span data-stu-id="0cf74-117">String</span></span>| <span data-ttu-id="0cf74-118">派生エンティティの ID。</span><span class="sxs-lookup"><span data-stu-id="0cf74-118">The ID for the derived entity.</span></span> <span data-ttu-id="0cf74-119">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="0cf74-119">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0cf74-120">関係</span><span class="sxs-lookup"><span data-stu-id="0cf74-120">Relationships</span></span>
<span data-ttu-id="0cf74-121">なし</span><span class="sxs-lookup"><span data-stu-id="0cf74-121">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0cf74-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0cf74-122">JSON representation</span></span>

<span data-ttu-id="0cf74-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0cf74-123">The following is a JSON representation of the resource.</span></span>

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
